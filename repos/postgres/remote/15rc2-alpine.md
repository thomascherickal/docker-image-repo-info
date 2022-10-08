## `postgres:15rc2-alpine`

```console
$ docker pull postgres@sha256:301f03506ad11c655e20a97cdd59254304ce51dbfbac5c922371e611283e871b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:15rc2-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:9791d2a5e509374a2e5a0db6dd9f48c8288524b1aebaff22d1ac57163ae205bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85354067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a0985adeebf5563034ff90da9de00befa955ff6eee07308f5281c499d8a161`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:10:45 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 01:10:45 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 01:10:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 01:10:45 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 23:54:44 GMT
ENV PG_VERSION=15rc2
# Fri, 07 Oct 2022 23:54:44 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Fri, 07 Oct 2022 23:57:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 07 Oct 2022 23:58:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 07 Oct 2022 23:58:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 07 Oct 2022 23:58:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 07 Oct 2022 23:58:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 07 Oct 2022 23:58:01 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Oct 2022 23:58:01 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Fri, 07 Oct 2022 23:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 23:58:01 GMT
STOPSIGNAL SIGINT
# Fri, 07 Oct 2022 23:58:01 GMT
EXPOSE 5432
# Fri, 07 Oct 2022 23:58:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ab741cca09cae3efd0bccbe57183973b177cda2b7f65d67078454dc1d97ba7`  
		Last Modified: Fri, 07 Oct 2022 01:30:44 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3636f308d36c203f3f75f1c294814f647b4641fc980b708edb341400491e6fc`  
		Last Modified: Fri, 07 Oct 2022 01:30:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869aae2b6e9db9ca3986d13ca4435a4ceb382c3eddddf65c59c5b8bb47ba5f23`  
		Last Modified: Fri, 07 Oct 2022 23:59:43 GMT  
		Size: 82.5 MB (82532060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd31985ccf75ab7b4f901541c2cf8127a2cd141bf3b3200d8be957ddc60e32a2`  
		Last Modified: Fri, 07 Oct 2022 23:59:32 GMT  
		Size: 9.5 KB (9453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12718e61353e7b95d520249121230a1b7c415a9b191950f4171eb8f894216db9`  
		Last Modified: Fri, 07 Oct 2022 23:59:32 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feb37ea0b051a47839a3df1bcc1194ea357eabaaee06e0ef554861405d1db54`  
		Last Modified: Fri, 07 Oct 2022 23:59:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b4fb0db53085f0267cb4bc28a084260499d3aaa109f7431c101e3bd7c253e`  
		Last Modified: Fri, 07 Oct 2022 23:59:32 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc2-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:2f6108c4ba351ec405c1a7a04d61123bc9e716439e6339da0ef1a1f6e888ee55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78548368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225edaefa42f71d9c805da1a74ddc20417d62606ee39db60d0934d37f8dee951`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 02:26:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 08 Oct 2022 02:26:56 GMT
ENV LANG=en_US.utf8
# Sat, 08 Oct 2022 02:26:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 08 Oct 2022 02:26:56 GMT
ENV PG_MAJOR=15
# Sat, 08 Oct 2022 02:26:56 GMT
ENV PG_VERSION=15rc2
# Sat, 08 Oct 2022 02:26:57 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Sat, 08 Oct 2022 02:36:29 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 08 Oct 2022 02:36:30 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 08 Oct 2022 02:36:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 08 Oct 2022 02:36:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 08 Oct 2022 02:36:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 08 Oct 2022 02:36:32 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 08 Oct 2022 02:36:32 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Sat, 08 Oct 2022 02:36:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 02:36:32 GMT
STOPSIGNAL SIGINT
# Sat, 08 Oct 2022 02:36:33 GMT
EXPOSE 5432
# Sat, 08 Oct 2022 02:36:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23716398dc3ba779f4482a6e7971806ab6a5bce9d412a2144f846b2866610613`  
		Last Modified: Sat, 08 Oct 2022 03:28:31 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dba6af302fa9533ac8ce701b19ea917fbe4ce219fbe85e9a27088fb3ab9b1a`  
		Last Modified: Sat, 08 Oct 2022 03:28:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b54fa9dd9953f54731fbc4209e2dcdebcf5a700fcc923d6bcd7e16267bd6087`  
		Last Modified: Sat, 08 Oct 2022 03:28:45 GMT  
		Size: 76.1 MB (76115350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb8b8753a052f0978d567b89ecba36799c854202685d4d3be864c302f500d20`  
		Last Modified: Sat, 08 Oct 2022 03:28:29 GMT  
		Size: 9.5 KB (9452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb188a6114fbf5971b98c1f8a88dc1d2f608063760f0b44e0eeabcdb1f8934`  
		Last Modified: Sat, 08 Oct 2022 03:28:29 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d024951ec27b876ed0f3a2ed130c8f1a72fb83b85e8f98d25d26141d8ce290c8`  
		Last Modified: Sat, 08 Oct 2022 03:28:29 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14f9f239be633de774aff7f4bae45811159fc3b32c7a4d1d38a06e17575e54`  
		Last Modified: Sat, 08 Oct 2022 03:28:29 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc2-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b2eab19616b2726ec7793f2b30f8915df10eeaac32c91c0925374c8303d9a838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84179210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe68bec911de9c443bb1eb6afb91633027dda9ceaf9927512fb14e94c9f9232b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:05:38 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 04:05:39 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 04:05:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 04:05:41 GMT
ENV PG_MAJOR=15
# Sat, 08 Oct 2022 00:41:11 GMT
ENV PG_VERSION=15rc2
# Sat, 08 Oct 2022 00:41:11 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Sat, 08 Oct 2022 00:44:51 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 08 Oct 2022 00:44:51 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 08 Oct 2022 00:44:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 08 Oct 2022 00:44:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 08 Oct 2022 00:44:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 08 Oct 2022 00:44:55 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 08 Oct 2022 00:44:57 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Sat, 08 Oct 2022 00:44:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:44:58 GMT
STOPSIGNAL SIGINT
# Sat, 08 Oct 2022 00:44:59 GMT
EXPOSE 5432
# Sat, 08 Oct 2022 00:45:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac05eb62a0d312c6a5077cc54b5bca58a2c51aec7a337f3339c7084aaf153c`  
		Last Modified: Fri, 07 Oct 2022 04:28:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbbc8b450549bfae843e4365be3315e577270effad7c627affbd83b95e98bad`  
		Last Modified: Fri, 07 Oct 2022 04:28:06 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c39ffa00f00dd7c43199d47d05f20aca1cd0aa5e6070d57ede09b465c3c695a`  
		Last Modified: Sat, 08 Oct 2022 00:47:49 GMT  
		Size: 81.5 MB (81455723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1a340d2ee473b4bb9e0605fbe91c248f11e5eaf21139d1e809c97f910972d4`  
		Last Modified: Sat, 08 Oct 2022 00:47:38 GMT  
		Size: 9.4 KB (9445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3532787c419d25e61c6401dcc1f56226b985d3ad43533497da6af4fb5b64a41`  
		Last Modified: Sat, 08 Oct 2022 00:47:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092cda714f3881c275e20c86a2f0d69e69bbebde9098c66b95c7b0a15b26be3b`  
		Last Modified: Sat, 08 Oct 2022 00:47:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f287b5e4c606afd5331b7ce3c823001117f08abd835785b346ae27c9604e4c`  
		Last Modified: Sat, 08 Oct 2022 00:47:38 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc2-alpine` - linux; 386

```console
$ docker pull postgres@sha256:c4baca5c67c20dca8c1113f6f821af72fb9a5c2c9ca69ca7724573f37608285b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90689152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ff80f6b600214c27efe0cd165e13bd9d19055c9d841ba544381dd4cbc5ff61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:58:32 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 06 Oct 2022 22:58:33 GMT
ENV LANG=en_US.utf8
# Thu, 06 Oct 2022 22:58:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 06 Oct 2022 22:58:35 GMT
ENV PG_MAJOR=15
# Sat, 08 Oct 2022 00:31:59 GMT
ENV PG_VERSION=15rc2
# Sat, 08 Oct 2022 00:32:00 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Sat, 08 Oct 2022 00:35:55 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 08 Oct 2022 00:35:55 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 08 Oct 2022 00:35:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 08 Oct 2022 00:35:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 08 Oct 2022 00:35:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 08 Oct 2022 00:35:59 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 08 Oct 2022 00:36:01 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Sat, 08 Oct 2022 00:36:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:36:02 GMT
STOPSIGNAL SIGINT
# Sat, 08 Oct 2022 00:36:03 GMT
EXPOSE 5432
# Sat, 08 Oct 2022 00:36:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0a2d06c52831b717922c82a177581313d43ff48fa82da49ed9fe0bf8002d8`  
		Last Modified: Thu, 06 Oct 2022 23:23:50 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3642389f32b5996f507baab5859e392131d7bce3768326935a4dfb51d4932b5a`  
		Last Modified: Thu, 06 Oct 2022 23:23:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3468a5b79751156563806610d1ce2f0b7e281b6e824f1d6b119fbfc8c9012e`  
		Last Modified: Sat, 08 Oct 2022 00:38:57 GMT  
		Size: 87.9 MB (87866197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c11699716e3af41f7e916107823bdaede19f872c6639d1f6106fa6cece43ce`  
		Last Modified: Sat, 08 Oct 2022 00:38:47 GMT  
		Size: 9.5 KB (9451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99070ea1cf6a5a8bd67b5cd2e07c8771493ac158b92f02adae945f4f0645bced`  
		Last Modified: Sat, 08 Oct 2022 00:38:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dbff24b1ddc7773a6106b2ea483f71a80eb4ee90dedf7f3e63831bc1671b64`  
		Last Modified: Sat, 08 Oct 2022 00:38:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328751f4c0a4a9eaea3cd00dcfca13a33e7c6389daef077c03f1ba5d7ea3a097`  
		Last Modified: Sat, 08 Oct 2022 00:38:47 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc2-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:e77ab9075f6f5eb9e0c894f27c9b94b6495d1f1fd436882ff6a13fbf028de3d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.6 MB (91648788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bb2de3301a202f1cf51b1973db7a8360222677e77cd66702c8e26cf03e7812`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:25:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 02:25:59 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 02:26:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 02:26:00 GMT
ENV PG_MAJOR=15
# Fri, 07 Oct 2022 23:57:53 GMT
ENV PG_VERSION=15rc2
# Fri, 07 Oct 2022 23:57:54 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Sat, 08 Oct 2022 00:02:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 08 Oct 2022 00:02:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 08 Oct 2022 00:02:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 08 Oct 2022 00:02:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 08 Oct 2022 00:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 08 Oct 2022 00:02:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 08 Oct 2022 00:02:27 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Sat, 08 Oct 2022 00:02:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:02:28 GMT
STOPSIGNAL SIGINT
# Sat, 08 Oct 2022 00:02:28 GMT
EXPOSE 5432
# Sat, 08 Oct 2022 00:02:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9886199ad194bb654781346f2cd4cce2905c90d143f8d77e5869dada1864c5`  
		Last Modified: Fri, 07 Oct 2022 02:54:28 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca1982ca555c7b16501b90c9ee856d6d3a531258352fd09a5db82ef45f9984`  
		Last Modified: Fri, 07 Oct 2022 02:54:27 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f84ba26038773c8a8508c4c19f3a1254d7d3342c253bbff72581ae3899fd37`  
		Last Modified: Sat, 08 Oct 2022 00:05:46 GMT  
		Size: 88.8 MB (88829514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd727fcc79a4db2579b281f9c6db94e190e5ef7a17248ff47d7bad366f3a97c3`  
		Last Modified: Sat, 08 Oct 2022 00:05:26 GMT  
		Size: 9.5 KB (9456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a0e611007d6e757c71656de47436a4c1488192ece3d2fb6bd9816d9c805c10`  
		Last Modified: Sat, 08 Oct 2022 00:05:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d2c847815f6764165a99f02e1407440f1ff399655c619f52330bc432c4033d`  
		Last Modified: Sat, 08 Oct 2022 00:05:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7869509d80e17201ce509499a3cdef1eb050f4dd18270786d0434862a60b74b9`  
		Last Modified: Sat, 08 Oct 2022 00:05:26 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15rc2-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:1bcc8e122ca7a3652c2eb344f794d430449f30b620bc7d7a48bbf6525daad71f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86556520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b915ebbe81b19d63c72876bd59b96f3cbdad5c5cdad6049430bad4642933a974`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:35:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Oct 2022 03:35:39 GMT
ENV LANG=en_US.utf8
# Fri, 07 Oct 2022 03:35:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 07 Oct 2022 03:35:41 GMT
ENV PG_MAJOR=15
# Sat, 08 Oct 2022 00:20:58 GMT
ENV PG_VERSION=15rc2
# Sat, 08 Oct 2022 00:20:59 GMT
ENV PG_SHA256=11739405e96699198733f4a0055362262c9c89f32d2e835e0b815687d700cc23
# Sat, 08 Oct 2022 00:25:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Sat, 08 Oct 2022 00:25:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Sat, 08 Oct 2022 00:25:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 08 Oct 2022 00:25:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 08 Oct 2022 00:25:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 08 Oct 2022 00:25:25 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 08 Oct 2022 00:25:25 GMT
COPY file:232dce6cf487afb0c0cc43d38932ff29614a74b57cd04557dc7398e6d2b93b8f in /usr/local/bin/ 
# Sat, 08 Oct 2022 00:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:25:26 GMT
STOPSIGNAL SIGINT
# Sat, 08 Oct 2022 00:25:26 GMT
EXPOSE 5432
# Sat, 08 Oct 2022 00:25:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e890de774640a358825541264ef983fef765c29d72f21038ede1ac41c85e6fd`  
		Last Modified: Fri, 07 Oct 2022 04:02:51 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310de1aaaef21df2d67997a7dfe754c704ddf70ece33ada85f4f2dd0a4e02359`  
		Last Modified: Fri, 07 Oct 2022 04:02:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ea36c603518ae0840ffd46af5bab0bbe1a0754f38f8613d5671de601d2f008`  
		Last Modified: Sat, 08 Oct 2022 00:28:36 GMT  
		Size: 83.9 MB (83949979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae215262e1808db624cf601bf433bb047239345fb5c40ff85e6ec6b4d406b444`  
		Last Modified: Sat, 08 Oct 2022 00:28:26 GMT  
		Size: 9.4 KB (9449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd232beae08388c82856432e7b4583883f1cb196a0056d680dc1bbd7a9aafa2`  
		Last Modified: Sat, 08 Oct 2022 00:28:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f4e864dc4397e63b0e2c6c662446d66b9f63a014a6d6ba586d05bf3bcff0c1`  
		Last Modified: Sat, 08 Oct 2022 00:28:26 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7124fffee2484e7a56d41c34cf8b03cac447ed2123ceeff121d388fafe7c1d`  
		Last Modified: Sat, 08 Oct 2022 00:28:26 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
