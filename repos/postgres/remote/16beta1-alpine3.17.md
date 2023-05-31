## `postgres:16beta1-alpine3.17`

```console
$ docker pull postgres@sha256:893704a444a8962690a18b217c5aa0c16324ce2fc5435f1b991631b280109fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `postgres:16beta1-alpine3.17` - linux; arm variant v6

```console
$ docker pull postgres@sha256:0be19694119c9e91fdd05b478c064e64f854cbf397b1014d0c88bd3c73eef797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94878344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83f94be1697577050215e9f033836401fba1d9f10b9c9d03405641cb45ad6285`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Fri, 07 Apr 2023 23:56:12 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 07 Apr 2023 23:56:12 GMT
ENV LANG=en_US.utf8
# Fri, 07 Apr 2023 23:56:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 31 May 2023 01:10:33 GMT
ENV PG_MAJOR=16
# Wed, 31 May 2023 01:10:34 GMT
ENV PG_VERSION=16beta1
# Wed, 31 May 2023 01:10:34 GMT
ENV PG_SHA256=59e248d434aa515fa2d31c0d161c4148f30d511dcde91f6e888684823b6849a8
# Wed, 31 May 2023 01:10:34 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 31 May 2023 01:15:32 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Wed, 31 May 2023 01:15:34 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Wed, 31 May 2023 01:15:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql
# Wed, 31 May 2023 01:15:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 31 May 2023 01:15:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA"
# Wed, 31 May 2023 01:15:37 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 31 May 2023 01:15:37 GMT
COPY file:e635913e9467265f505455bc3f08bed37d67ce6597a1f10365f8faf79f09b654 in /usr/local/bin/ 
# Wed, 31 May 2023 01:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 May 2023 01:15:38 GMT
STOPSIGNAL SIGINT
# Wed, 31 May 2023 01:15:38 GMT
EXPOSE 5432
# Wed, 31 May 2023 01:15:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbeb693b3ad51663da3d7f481eff1783f58e2ffe548d9f5e1212c4d61f49415`  
		Last Modified: Sat, 08 Apr 2023 00:13:50 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d67b90e3c302b3ab64223a61b68243861566a39eb53d3fbd780e7402b0b8c6`  
		Last Modified: Sat, 08 Apr 2023 00:13:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78710b686c5d11717ecfa40c241066289ec857a9aa57b8157bacfaeeaecf6aa`  
		Last Modified: Wed, 31 May 2023 01:17:09 GMT  
		Size: 91.8 MB (91751397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82517c8dcc6dada1f1f0d395f88f79501babd866889e3015c67ee63b33470e38`  
		Last Modified: Wed, 31 May 2023 01:16:54 GMT  
		Size: 9.6 KB (9571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20739a033bbaea191edab532088526912e1ca6bec8ad6a3a784c2dee000df4d9`  
		Last Modified: Wed, 31 May 2023 01:16:54 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1349f2409d64f9bce940f9f09ce51def8d909628f9869e25995324d8c90df763`  
		Last Modified: Wed, 31 May 2023 01:16:54 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f728ac43cc45b8917b30da86281253130cee5579b4d50ce41b66fb79400a5`  
		Last Modified: Wed, 31 May 2023 01:16:54 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
