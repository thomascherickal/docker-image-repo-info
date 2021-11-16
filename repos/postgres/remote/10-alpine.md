## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:adab1b329d5b734e9bbae35b262d95027f04801e2747a0a65d9d6c55581e7a2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:10-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:1d132a36102c19718d225094b493bb363728c3a2c86c2d9cf6abc1fce573867e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.2 MB (30176842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f48f126361d3cb8df2fefc629c4278954b3435802b7c7e557529743ae801e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:06:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 13 Nov 2021 05:06:01 GMT
ENV LANG=en_US.utf8
# Sat, 13 Nov 2021 05:06:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 13 Nov 2021 05:33:18 GMT
ENV PG_MAJOR=10
# Sat, 13 Nov 2021 05:33:18 GMT
ENV PG_VERSION=10.19
# Sat, 13 Nov 2021 05:33:18 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 01:46:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 01:46:20 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 01:46:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 01:46:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 01:46:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 01:46:22 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 01:46:23 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 01:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 01:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 01:46:24 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 01:46:24 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 01:46:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f97b97dbe44d3d5922703b0d43a419416f14f7acfda692d113a7aa9b9721fe1`  
		Last Modified: Sat, 13 Nov 2021 05:43:31 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b95022c44c584684bb06e7baad164584f8952fb082bab4a0daf8dc9c4b803dd`  
		Last Modified: Sat, 13 Nov 2021 05:43:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f4969648c1c572ea27f0a7cd3c48b280bc9d6581cd472667df85c02934f3a4`  
		Last Modified: Tue, 16 Nov 2021 01:57:45 GMT  
		Size: 27.3 MB (27339504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873087b046a30b84bfdaf0e8353a556fabd0b8eff8066f26cb1a0dc5e951b015`  
		Last Modified: Tue, 16 Nov 2021 01:57:38 GMT  
		Size: 7.7 KB (7731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a6d947c2c198ea8de758660b6d66cb4199ba632c15c3bd04692822cae62d35`  
		Last Modified: Tue, 16 Nov 2021 01:57:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6794ec70f65d39fecfbad50714de02b51f905d6a9ed4c54176c67ccde6eb88f`  
		Last Modified: Tue, 16 Nov 2021 01:57:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4315d91b89ea549cb795a2e7432e5edacb786aaec75e226a3fe13dffadbe05b9`  
		Last Modified: Tue, 16 Nov 2021 01:57:38 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ee0bc35333f74d1b1c631727cb3827cd0263e68c7acdf57a10e7a89a196f3`  
		Last Modified: Tue, 16 Nov 2021 01:57:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:f5e7e28a8be6e48f8725b19dde798c2a553624da9eb77ef033f74e96ba48cac0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 MB (29229315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a54fe5c56374021a8e67dd4b122817829a63e5686a653894bf8814f2434502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:23:41 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 13 Nov 2021 00:23:42 GMT
ENV LANG=en_US.utf8
# Sat, 13 Nov 2021 00:23:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 13 Nov 2021 00:44:48 GMT
ENV PG_MAJOR=10
# Sat, 13 Nov 2021 00:44:48 GMT
ENV PG_VERSION=10.19
# Sat, 13 Nov 2021 00:44:49 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 02:14:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 02:15:01 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 02:15:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 02:15:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 02:15:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 02:15:06 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 02:15:06 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 02:15:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 02:15:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 02:15:09 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 02:15:09 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 02:15:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306bf867c1af5e86348eac10e572e5bbf7b1df7161b3237e6dbf067420ba562`  
		Last Modified: Sat, 13 Nov 2021 00:54:50 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b273647972e23088da4f0aa3896b1e39e9c26c17f7239fe3fa6ca165b5190765`  
		Last Modified: Sat, 13 Nov 2021 00:54:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc4df9b303b153deaf36977a5983b9794427217b0b257804e7267256cc43e3a`  
		Last Modified: Tue, 16 Nov 2021 02:28:23 GMT  
		Size: 26.6 MB (26579571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a82749776a581baad0b7baac70bea2085b2c80cbfafc91343f92729dcb556e4`  
		Last Modified: Tue, 16 Nov 2021 02:28:04 GMT  
		Size: 7.7 KB (7725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5582cb0ca836fe74472c5fc1c7fcd5a7468816802cfcb758b5d282e6d2866a7a`  
		Last Modified: Tue, 16 Nov 2021 02:28:04 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54233a48618b077aa2f342c5def208b66c7386aa48fef6c35f1e39d8909ac45b`  
		Last Modified: Tue, 16 Nov 2021 02:28:04 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7621fb169440343f737818600c4aeba3b9ee328a6abd8e569fc753cdc7fa91b0`  
		Last Modified: Tue, 16 Nov 2021 02:28:04 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0729cd6a154c828e5cc9733b0fcb605c7dcd65ca48a022a6aaaddedc100072`  
		Last Modified: Tue, 16 Nov 2021 02:28:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:da7b7764ea863f23e5f726231998607b0dc5e529e2c04fea3de96bbbbec55bf5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28039886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881a9a7b5135eb82f924b73fb8a3522243e5d185fd39ebe7b380f78130f43e94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:25:42 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 12 Nov 2021 20:25:42 GMT
ENV LANG=en_US.utf8
# Fri, 12 Nov 2021 20:25:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 12 Nov 2021 20:46:48 GMT
ENV PG_MAJOR=10
# Fri, 12 Nov 2021 20:46:48 GMT
ENV PG_VERSION=10.19
# Fri, 12 Nov 2021 20:46:49 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 02:31:46 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 02:31:48 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 02:31:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 02:31:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 02:31:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 02:31:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 02:31:52 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 02:31:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 02:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 02:31:55 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 02:31:55 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 02:31:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65aac23bae9dde4628b949f53b16460bf45bbe0cb93feb0ca4e699560ec405be`  
		Last Modified: Fri, 12 Nov 2021 20:59:27 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c82e83b49adac505e95de3db74b7b3d754078880f57793b8cd1a81d5c456289`  
		Last Modified: Fri, 12 Nov 2021 20:59:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b21ead03e56567523a720f4fb85fb78d0cb629dcbd7dd8b3d3e59d69c1d55f`  
		Last Modified: Tue, 16 Nov 2021 02:48:02 GMT  
		Size: 25.6 MB (25586906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e40c1b36b4b58dfc5b02d29a63127a12035f7f97cde04b6e7b3695a1e32cc4`  
		Last Modified: Tue, 16 Nov 2021 02:47:45 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb2bac28e8a5027300b7f62fc2cd49f1d6faa5bcdd8f039df0dd150e0d79a35`  
		Last Modified: Tue, 16 Nov 2021 02:47:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a335be964f0058f701bcac22bd4999d5856493dfae48374c292eb426219c5`  
		Last Modified: Tue, 16 Nov 2021 02:47:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25faba695f53e049779bc4b7be0f578e3a2ac40b8a5874690e8c5653da8b40b`  
		Last Modified: Tue, 16 Nov 2021 02:47:45 GMT  
		Size: 4.7 KB (4722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8309fd104157db392537ece9a3ab8ff68a802b85313ffbd34f194ab55e5429`  
		Last Modified: Tue, 16 Nov 2021 02:47:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:bfd0c0d94a240217ee31ebc64e0c69a9ff4e2f95b15f3133ed56eef7ee64f680
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29875412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc400149b9df1cb6f3944d4369d6390e78945b555c26408342697089d318fd5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:41:51 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 12 Nov 2021 23:41:52 GMT
ENV LANG=en_US.utf8
# Fri, 12 Nov 2021 23:41:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 13 Nov 2021 00:01:09 GMT
ENV PG_MAJOR=10
# Sat, 13 Nov 2021 00:01:10 GMT
ENV PG_VERSION=10.19
# Sat, 13 Nov 2021 00:01:11 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 02:09:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 02:09:28 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 02:09:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 02:09:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 02:09:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 02:09:32 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 02:09:34 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 02:09:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 02:09:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 02:09:36 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 02:09:37 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 02:09:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736fbb41a17a3d331434d1ced1bbefaf60ce58df545c90a6d1dbfeec5eb9af41`  
		Last Modified: Sat, 13 Nov 2021 00:10:26 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99566057aebae6d994d20c6ed9fa0b7e7cd103f58ddce64c9096b244ec9905a0`  
		Last Modified: Sat, 13 Nov 2021 00:10:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a9477ed5d952482146c366d321e1bdfb49429a0839b7c9fa1e868af4bfa4c`  
		Last Modified: Tue, 16 Nov 2021 02:18:56 GMT  
		Size: 27.1 MB (27143474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e397c967f032eb1a69489ffaad4b3643c1c2c4a79ed57a6593610be164db26`  
		Last Modified: Tue, 16 Nov 2021 02:18:50 GMT  
		Size: 7.7 KB (7729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24ef8e62ac9b81c8d613ac0506623c6359830f654bba9eaabf3e323f7c3d504`  
		Last Modified: Tue, 16 Nov 2021 02:18:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d288339a2aa75b5cf90ae09cf7c2aa6bc298535a6cff6ed38cfd78cf26f711d1`  
		Last Modified: Tue, 16 Nov 2021 02:18:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ed396452e99ee1937697f2fc95b9ba156ebe2f2723af646275158e1c5e0202`  
		Last Modified: Tue, 16 Nov 2021 02:18:50 GMT  
		Size: 4.7 KB (4718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450ececc7097801a1029bac8af979d4b3dc4e7389df6eb2251782e5e085e6433`  
		Last Modified: Tue, 16 Nov 2021 02:18:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:2e112607cb48e0672e6216f24fb4cf9cf4ee54879fddf71e956ec54a3361b38a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31195482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41d8c325251bbb9bc8a6f75f261110a4c819ad3e85ff4a8ea441570ce6711ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 23:55:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 12 Nov 2021 23:55:01 GMT
ENV LANG=en_US.utf8
# Fri, 12 Nov 2021 23:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 13 Nov 2021 00:27:00 GMT
ENV PG_MAJOR=10
# Sat, 13 Nov 2021 00:27:00 GMT
ENV PG_VERSION=10.19
# Sat, 13 Nov 2021 00:27:01 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 02:16:11 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 02:16:12 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 02:16:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 02:16:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 02:16:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 02:16:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 02:16:14 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 02:16:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 02:16:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 02:16:16 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 02:16:16 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 02:16:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69c9882c88ce94760f0d36deed4d8f55228d1df726a3bc33021031f8922aa5a`  
		Last Modified: Sat, 13 Nov 2021 00:41:13 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2788bc110cff8f1594e3fabf8ae849a646240d7e3c7ce77b566583c4a66b5467`  
		Last Modified: Sat, 13 Nov 2021 00:41:13 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91fd24bc1758e653639619efaea9cbbac5563b76c78d1a415ada278cd33a04b`  
		Last Modified: Tue, 16 Nov 2021 02:26:37 GMT  
		Size: 28.4 MB (28350181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbef6f49382581251b5657355b491bf35bab9f639a6caaa70609a00f1af70a`  
		Last Modified: Tue, 16 Nov 2021 02:26:30 GMT  
		Size: 7.7 KB (7726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4ecc4d1ef1972c669fd01847d5d9c82cb860ba00c7f15b03db762b3b6b26c9`  
		Last Modified: Tue, 16 Nov 2021 02:26:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad3a166719ed19c2ebd6f67518498ba1b35adcfdc0c927a0dc399ba5fbe1478`  
		Last Modified: Tue, 16 Nov 2021 02:26:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a86c36a103c52c8a3e891ef41292a6694a35bc9402fb98ce10df32d4367be`  
		Last Modified: Tue, 16 Nov 2021 02:26:30 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b3e57bb73895e9a6c771d57a45aab1ead87187569c14bb5b6e647f159d5174`  
		Last Modified: Tue, 16 Nov 2021 02:26:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:5db415aa7cd991d05a3ba46b8a0dc115133a6f40c7f04163cec59a5348709455
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (29984927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c14b4cca8fd10c551469a901d72355fd1f0ccda40b5ac5d6fbda96887ee2264`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 14:19:29 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 13 Nov 2021 14:19:31 GMT
ENV LANG=en_US.utf8
# Sat, 13 Nov 2021 14:19:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 13 Nov 2021 14:43:42 GMT
ENV PG_MAJOR=10
# Sat, 13 Nov 2021 14:43:46 GMT
ENV PG_VERSION=10.19
# Sat, 13 Nov 2021 14:43:50 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Sat, 13 Nov 2021 14:46:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 13 Nov 2021 14:46:50 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 13 Nov 2021 14:46:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 13 Nov 2021 14:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 13 Nov 2021 14:47:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 13 Nov 2021 14:47:10 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 13 Nov 2021 14:47:11 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Sat, 13 Nov 2021 14:47:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 13 Nov 2021 14:48:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:48:42 GMT
STOPSIGNAL SIGINT
# Sat, 13 Nov 2021 14:48:49 GMT
EXPOSE 5432
# Sat, 13 Nov 2021 14:48:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e892d223635db5048d4e0f826cfa9094090c3aa12a15afc7fdd249d076ca3e80`  
		Last Modified: Sat, 13 Nov 2021 14:54:39 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443b2a29145c872139ba01a0f2ab1a45f154e89a612cdd03ded00d39d7e4875`  
		Last Modified: Sat, 13 Nov 2021 14:54:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0400f356fc33acd13b2fb091c90696f9eabd0c091f150496d695d931e8fbee36`  
		Last Modified: Sat, 13 Nov 2021 14:57:03 GMT  
		Size: 27.2 MB (27153101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c3d5f46445843a0bf3ff2ab41e9b7c9ce9029157a4d7c74e91cc7d1394862f`  
		Last Modified: Sat, 13 Nov 2021 14:56:56 GMT  
		Size: 7.7 KB (7732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7546c2d01af87748dfec0fcb61f51155b4e5fd7d3f6874ca805ec9940c95c07`  
		Last Modified: Sat, 13 Nov 2021 14:56:55 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc90dd64742b32c83d16fe34de9ba8f9e4311dba244628e9c33dd5aa5acd5d7`  
		Last Modified: Sat, 13 Nov 2021 14:56:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012ad265685acc3b0f03212006534f403e615771ed1b32f96c56103c4d3d2c09`  
		Last Modified: Sat, 13 Nov 2021 14:56:55 GMT  
		Size: 4.7 KB (4715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cd03722709e38d255ed523d7d637d92a8a689b370d2055bf42e81d67ac9bbb`  
		Last Modified: Sat, 13 Nov 2021 14:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:980a15dbbcb9b1fc45f2fb251ac03887b9ec297ee49c8be3da396b703d022199
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30057197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4625eb63ef236b65c17b846d102b72218548fa34d7b0cede180c8fcc63e5fb22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:02:11 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 12 Nov 2021 19:02:11 GMT
ENV LANG=en_US.utf8
# Fri, 12 Nov 2021 19:02:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 12 Nov 2021 19:14:10 GMT
ENV PG_MAJOR=10
# Fri, 12 Nov 2021 19:14:10 GMT
ENV PG_VERSION=10.19
# Fri, 12 Nov 2021 19:14:10 GMT
ENV PG_SHA256=6eb830b428b60e84ae87e20436bce679c4d9d0202be7aec0e41b0c67d9134239
# Tue, 16 Nov 2021 01:57:43 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-utils 		perl-ipc-run 		perl-dev 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 16 Nov 2021 01:57:44 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 16 Nov 2021 01:57:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 16 Nov 2021 01:57:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 16 Nov 2021 01:57:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 16 Nov 2021 01:57:46 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 16 Nov 2021 01:57:46 GMT
COPY file:7bb2d643a5007a2573ce85b55b80b2ddaa7af3a038cba459ffbf2e367376ca53 in /usr/local/bin/ 
# Tue, 16 Nov 2021 01:57:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 16 Nov 2021 01:57:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Nov 2021 01:57:47 GMT
STOPSIGNAL SIGINT
# Tue, 16 Nov 2021 01:57:47 GMT
EXPOSE 5432
# Tue, 16 Nov 2021 01:57:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11d0e178e11b961bdeb7fbf4c5d37bdf95bead1a94bf7cb11c22318da7b0408`  
		Last Modified: Fri, 12 Nov 2021 19:19:45 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013949685d6dbf2034fe35128fa32dead6dda85c74b516d4e075450693ad8cd7`  
		Last Modified: Fri, 12 Nov 2021 19:19:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db451e018401ae3da050724b28598e180c0abd37f2d6615ba14f43e5a7529c9c`  
		Last Modified: Tue, 16 Nov 2021 02:04:12 GMT  
		Size: 27.4 MB (27433560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335d0149fb8ba44f65d2175561d469b8c533eef44da6b51ff41bed9c7c9bf01b`  
		Last Modified: Tue, 16 Nov 2021 02:04:07 GMT  
		Size: 7.7 KB (7730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362f31ed77c6819e0a50f5dfae85c55fef192aaaed0645e5ec0d8a7e47c0f806`  
		Last Modified: Tue, 16 Nov 2021 02:04:07 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad5115bd32b61d6755a0492467395f0f0cc4d52cf275fd57d1f9470ab5ff227`  
		Last Modified: Tue, 16 Nov 2021 02:04:07 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5280052c2a9691495863314d290db8f92723b9150d60b396c8012cc02aeae546`  
		Last Modified: Tue, 16 Nov 2021 02:04:07 GMT  
		Size: 4.7 KB (4718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f213676eec6df2f8ebeec4890b1c838874765d348b299caa00e2d39b548cf7`  
		Last Modified: Tue, 16 Nov 2021 02:04:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
