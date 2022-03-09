## `postgres:14-alpine`

```console
$ docker pull postgres@sha256:126bcff3a868d6bc79fbd9588e276731fa634f7137dd447476662da9d655ddfc
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

### `postgres:14-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:e181ba2f69f24c58f057a0eef7e66baf2f5dce76ee7af416407b226b4cce2b24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83304798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad69bf1fc05822f5e3eab4c6b56088329a6862c1f9b2fbf5fb0ebf6b5a3a1a8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:59:34 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:59:34 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:59:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:59:35 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:28:16 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:28:17 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 19:40:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 19:40:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 19:40:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 19:40:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 19:40:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 19:40:30 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 19:40:30 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 19:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 19:40:31 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 19:40:31 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 19:40:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e01d57241cf7ef93a91060f5eb0b895a4b443f20dc1ce5e77d441184a6dc2`  
		Last Modified: Tue, 30 Nov 2021 05:48:55 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0646b0f1eadaf0cd3fdb4c4490a69c4c7aed9b7ae10b24eb9005c59aa0b6e57`  
		Last Modified: Tue, 30 Nov 2021 05:48:55 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d8a6193e8a2a9ec1ed2e7a5b29a90cf6c601e2ff6aa9eca4b7a9b35669de8e`  
		Last Modified: Tue, 08 Mar 2022 20:07:22 GMT  
		Size: 80.5 MB (80470702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4294ad891cb675643fc889c2e1e3ce515710ba4ca6ab31d01c1ac8404c60c5c1`  
		Last Modified: Tue, 08 Mar 2022 20:07:08 GMT  
		Size: 9.2 KB (9200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44eb3e67c359c63a09e8d12e0b0ba3b97a165b37ce42b000b3005749b3579812`  
		Last Modified: Tue, 08 Mar 2022 20:07:08 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ed689d95a09d7663a9993f4a1f38f77e7ef243e4e306edaa27edcd4e2b7c6`  
		Last Modified: Tue, 08 Mar 2022 20:07:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdb0015416e246b4355d4a7447255bb9c8c08deba5ce9f137940fdda962bc35`  
		Last Modified: Tue, 08 Mar 2022 20:07:08 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:6f2b11d69b6b14df322d139f2911e67f1bbe6abc4cd738ea180c6712b9c675a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81014671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c43c723b61a0f763a54ac0ba79ad28b22d164854c88fa2b87101de6770912b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:39:17 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:39:18 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:39:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:39:20 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:01:01 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:01:02 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 20:22:13 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:22:15 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:22:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:22:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:22:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:22:19 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:22:19 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:22:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:22:20 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:22:21 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:22:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a865398e355d4d5f58fd1b16748daf1827598bdf1ba26c1d38fa7c8370d6705c`  
		Last Modified: Tue, 30 Nov 2021 05:15:02 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d879fc486c1bcf6d31fd2a8a5a4bc14acf4cc6f2d73e99dbf611ea8532bf4685`  
		Last Modified: Tue, 30 Nov 2021 05:15:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e8dacd7c63b8be13daa5db9988bab2ec0f005a3d48651501770bac7e92a276`  
		Last Modified: Tue, 08 Mar 2022 20:44:49 GMT  
		Size: 78.4 MB (78367561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951832e67ee005f61e64b0e80dea11d929c81469267e16eb721f3e7603af324e`  
		Last Modified: Tue, 08 Mar 2022 20:44:03 GMT  
		Size: 9.2 KB (9203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a2864332b291ec036aff9bdc0cea7612c3d60712e3dd8dedbe547a6b8db92e`  
		Last Modified: Tue, 08 Mar 2022 20:44:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23ce236225ba1ca303961ee52a66e3470fb76bef84717f6573a2f8be9998fcd`  
		Last Modified: Tue, 08 Mar 2022 20:44:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1e4ff0d63e4ea00231cc4e102906addc6e65c21fc74dde5965ff4f7267fc8d`  
		Last Modified: Tue, 08 Mar 2022 20:44:03 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:b367bcdfa3026aa3605c9cd95abb4ee37b8be1f7a7f078718c5c31a1056ebb83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76295728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3537f60ba066870de143ca557594d565188bbc242ccddd5058477c0fd415fdc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:45:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 07:45:15 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 07:45:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 07:45:17 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:46:42 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:46:42 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 20:52:54 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:52:56 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:52:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:52:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:53:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:53:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:53:01 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:53:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:53:01 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:53:02 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:53:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f681d006162b865bd7dca8476d129c7fa1193b246ad8a598d27eb28769a6ac`  
		Last Modified: Tue, 30 Nov 2021 12:10:30 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eb577cd41aefd27e490e1cbe04812996920ee2af42f358c659d1bb8a40230`  
		Last Modified: Tue, 30 Nov 2021 12:10:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7aafd56f3af4d0e32218b7be816d5a09dcd83e2b8b79b7f434365dd49a39c36`  
		Last Modified: Wed, 09 Mar 2022 00:03:08 GMT  
		Size: 73.8 MB (73845278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224edcd719fe82d63a51df3ff3e354ceb44690536e3c24b449720519ba970789`  
		Last Modified: Wed, 09 Mar 2022 00:02:28 GMT  
		Size: 9.2 KB (9202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc8490a3f94a15d68d5dbc00ad5efc3b61a05cd3bc5fe357dbe6cd5e9e8abea`  
		Last Modified: Wed, 09 Mar 2022 00:02:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104b17039316dda85e154adb65a9a0c6759532afece337b1e500f3ad9ea404c`  
		Last Modified: Wed, 09 Mar 2022 00:02:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975c8a1194bc548ac987a141b9fcc883c14e6d6dbc00cf91a77085925a7d3e`  
		Last Modified: Wed, 09 Mar 2022 00:02:28 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2908dfde81ee7f6fb61eeab1609dda8010aaa75a8d8d433fbbe24f09d1eddd5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (82005048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c2c60cb0185370e67f6e92eadc921e63405ee0631101463fff19de0daebb8df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:27:18 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:27:19 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:27:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:27:21 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:48:18 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:48:19 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 19:58:22 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 19:58:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 19:58:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 19:58:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 19:58:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 19:58:27 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 19:58:29 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 19:58:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 19:58:30 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 19:58:31 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 19:58:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995a68b04f2b01f2160f500ef732a967a427af5da712fac9029eeecbc80af73d`  
		Last Modified: Tue, 30 Nov 2021 05:22:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a8bdf2ee5e8b95fdba44140b8595c955b8639595bcf5c0f15841330176d8e5`  
		Last Modified: Tue, 30 Nov 2021 05:22:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb18a88cc10c074e6b58a60134c019ce626e14092e6c02c5cdb981b4480f6d9`  
		Last Modified: Tue, 08 Mar 2022 20:36:30 GMT  
		Size: 79.3 MB (79274033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc571f03fdc447cf8c910a0da9f2f090b6a19b7e139c43925bd531e734e4ee68`  
		Last Modified: Tue, 08 Mar 2022 20:36:19 GMT  
		Size: 9.2 KB (9205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd8569e8cc9a559f9ec0e1c91337cf97813868bea503d127f5a51ff47b5c1c`  
		Last Modified: Tue, 08 Mar 2022 20:36:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5e941f6d744fe5956e80a2d59e2bcd81eabe20f8295fd73f7f21c2762e04f9`  
		Last Modified: Tue, 08 Mar 2022 20:36:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eabdceb69dfa8a1e3d60a85d659db4db60ddff221bd317cc7ce4679ffd3a74`  
		Last Modified: Tue, 08 Mar 2022 20:36:19 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; 386

```console
$ docker pull postgres@sha256:36993407546ccfd6611f5682b3f2346d3e86b0c9202d3f16e8770aeb58f7e288
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88194836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6d1910f8c6f50adf24c10285d502d1b7aa1851d81e9c7185a9c868883be0ccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:41:28 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 02:41:28 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 02:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 02:41:29 GMT
ENV PG_MAJOR=14
# Fri, 11 Feb 2022 23:50:46 GMT
ENV PG_VERSION=14.2
# Fri, 11 Feb 2022 23:50:46 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 20:12:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:12:54 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:12:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:12:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:12:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:12:56 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:12:56 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:12:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:12:56 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:12:56 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:12:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af56146d51f459d9baa843fcf88ab0b80c1c9de99248bc2163f19197ba95d05`  
		Last Modified: Tue, 30 Nov 2021 04:43:41 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a14412d0e45405abe51e591c8467d465e5f91db0600bf8b9120d9c6f15217c`  
		Last Modified: Tue, 30 Nov 2021 04:43:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627445d42188d6d264baff125193ab309289a26086e3aaca6ab98d40e9809d09`  
		Last Modified: Tue, 08 Mar 2022 21:19:17 GMT  
		Size: 85.4 MB (85352038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9706f97d3759b12d083a5b27ec9cec16dd09d7c67564a08bc7107a64fad2a67`  
		Last Modified: Tue, 08 Mar 2022 21:18:59 GMT  
		Size: 9.2 KB (9204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bff1e4407b94d7b96555af06e1f46fa280a5d1b55dc300d56dd6fb7d17899d9`  
		Last Modified: Tue, 08 Mar 2022 21:18:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e43df45c810693b63392ef9e39791163057c7340c43626b9bb6b027c1a4d0`  
		Last Modified: Tue, 08 Mar 2022 21:18:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd362fba40ae4754d9743a6e7cbba0489a589589897b8d13676d4d60aa93f06`  
		Last Modified: Tue, 08 Mar 2022 21:18:59 GMT  
		Size: 4.7 KB (4694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:0fbe64d9914357b6b5ecf62e4cbf277e174c087294b184cde95561960d994ec9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.6 MB (88600884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19755b82a3e6b4a120e1bf90203d52acab4344aeb54cc3e2be2037d241d3245e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:26:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:26:53 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:27:08 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:03:21 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:03:25 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 20:31:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:31:45 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:31:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:31:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:31:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:32:03 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:32:06 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:32:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:32:12 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:32:15 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:32:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21143ce0a44ab602b12471d2a1cf95c5dcbc9d805bd8ede00e2766f24d295b5`  
		Last Modified: Tue, 30 Nov 2021 05:10:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c45529781f9e932a9022851fca78ba53022920657aa14e0479b195cac40189`  
		Last Modified: Tue, 30 Nov 2021 05:10:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8a62e3a252042f932cd73931a5253bd422996b84aba37d701a5563502ab376`  
		Last Modified: Tue, 08 Mar 2022 21:08:56 GMT  
		Size: 85.8 MB (85770408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a11454593b750797bc2a2ff7e5e256f3e2114b39a223779150beb58123649ce`  
		Last Modified: Tue, 08 Mar 2022 21:08:42 GMT  
		Size: 9.2 KB (9207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8488b39a83468b6273af047e96939538482e551ffe67da58e97548e23bcafd1c`  
		Last Modified: Tue, 08 Mar 2022 21:08:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6a66c3a6a7ef280055e9b1726d4fe8976d73dfa0edd6184268e0b3a7010b38`  
		Last Modified: Tue, 08 Mar 2022 21:08:42 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5447987f38f7e814e59d5fcd70a859d16973ac2954a274fea9020677eaa7780`  
		Last Modified: Tue, 08 Mar 2022 21:08:42 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:23ca1f15756484920ce898f185f6af33f2826de74b765ef8407dfb47126b23fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84357187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a831194a15ca4509730a29fb2844f01fe466ac0617179195b0e04d16f31a1c95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 08:50:09 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 08:50:09 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 08:50:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 08:50:10 GMT
ENV PG_MAJOR=14
# Sat, 12 Feb 2022 00:00:29 GMT
ENV PG_VERSION=14.2
# Sat, 12 Feb 2022 00:00:29 GMT
ENV PG_SHA256=2cf78b2e468912f8101d695db5340cf313c2e9f68a612fb71427524e8c9a977a
# Tue, 08 Mar 2022 19:58:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 19:58:40 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 19:58:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 19:58:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 19:58:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 19:58:41 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 19:58:41 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 19:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 19:58:42 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 19:58:42 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 19:58:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96844042cfb587d09e525bf6890e267412ad5971e27ece4faa02e82f6fda3c87`  
		Last Modified: Tue, 30 Nov 2021 09:46:44 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ee6a78ec06ec30a73acc9c0f2337f744b77da2931a6e0c1d3efb35d76cfe6`  
		Last Modified: Tue, 30 Nov 2021 09:46:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3c64fbc3e2606f76e8dbdc3e56d1fa5445188a1a161faec4be6603e65e2bed`  
		Last Modified: Tue, 08 Mar 2022 20:44:31 GMT  
		Size: 81.7 MB (81735550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881bb1418a62303cee6d1df39ae4f52e2add5d9f2f59d9d3be15a8a3da476c3c`  
		Last Modified: Tue, 08 Mar 2022 20:44:23 GMT  
		Size: 9.2 KB (9207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54527417c22b6bd5d83ead64fbd78255e95f194e91b400c9cb2c65a3ff6338ed`  
		Last Modified: Tue, 08 Mar 2022 20:44:23 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f37c7faf92ae82ece6d8c4b7d0c3cb7c50a893eb9ef1c813c2bc5ca901df2c`  
		Last Modified: Tue, 08 Mar 2022 20:44:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bf80b7fa469a98638d648216b3477a203c5de21ac0b4fea226182085248253`  
		Last Modified: Tue, 08 Mar 2022 20:44:22 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
