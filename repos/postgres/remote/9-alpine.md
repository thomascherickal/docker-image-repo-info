## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:0927ac1a17d8404e65a4ecd4d2135e27742f512ced6d0a60c9e5802712ade21d
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
$ docker pull postgres@sha256:f4f711f83e7bcda6874cc2420c74a020bfc16ea3226ab946bc119c8fd1eb35f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14487307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d5adc750f3a785575cbe26b9652f8cffbb96acc1de845872901a3a9e10d01dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:59:48 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 00:59:49 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 00:59:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 01:25:40 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 01:25:40 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 01:25:40 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Thu, 17 Dec 2020 01:29:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 01:29:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 01:29:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 01:29:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 01:29:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 01:29:39 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:23:01 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 01:23:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:23:02 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:23:02 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:23:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8392b19747a95c5f0945f923608970a15320af8654f0a299a0fc345f7d2aa926`  
		Last Modified: Thu, 17 Dec 2020 01:35:47 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae408abf9c34442cb63539f6995aa2f7a7f934c7671d59879da83a8a0d936c6d`  
		Last Modified: Thu, 17 Dec 2020 01:35:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6fd3c3a24b0af857fe772afef8af0ed4ec959a89136730cdb8c6ea4b65345c`  
		Last Modified: Thu, 17 Dec 2020 01:37:10 GMT  
		Size: 11.7 MB (11674913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8374e9a251e3b6019c114559a4d71ae7705fe831bb3ad6dcc5636bb703649ca6`  
		Last Modified: Thu, 17 Dec 2020 01:37:06 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3ce0d8901ef660d769de443ec934b1f4e23fcdc69d9be235a4884a255e7641`  
		Last Modified: Thu, 17 Dec 2020 01:37:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67571031a24b47fb783aa79507ded3c98035ba12478bd5249c97ba6bb746e78e`  
		Last Modified: Thu, 17 Dec 2020 01:37:06 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2154a17dcc2e060aa087eff5aa1dad55cccd3dd2c17bea4c3a0717d36e3815d`  
		Last Modified: Wed, 30 Dec 2020 01:24:40 GMT  
		Size: 4.4 KB (4390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ed4ce7aae1a65452827641a7dc15cb4103feb9dc99a0a2162b3406be5f133d`  
		Last Modified: Wed, 30 Dec 2020 01:24:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:6b6bc5de6f1be99f76784126b1b7bef3d12a5ee5a804ffb8b372e5bb8a5435fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13842596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae974a9b6df7ad12d2db7b44cefc1f4280caa68cb5853708b84dcfa9bf6908b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:45:15 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:45:16 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:45:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 06:01:34 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 06:01:39 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 06:01:40 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Fri, 18 Dec 2020 20:44:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 20:44:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 20:44:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 20:44:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 20:44:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 20:44:21 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:55:48 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:55:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:55:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:55:54 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:55:56 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:55:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8281cbd4bde01cbf0ed0e8ecf5550798d848c1d7d2d642a0416759d8df635f3`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae834cabab68fcc6ee1f251914773d8111eba34640f8849961845844a4f4681`  
		Last Modified: Thu, 17 Dec 2020 06:08:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa20e9ce5db992d499d25f1e6712bec6c3b84a6a00ee3a59a57926bd1d15f18a`  
		Last Modified: Fri, 18 Dec 2020 20:48:26 GMT  
		Size: 11.2 MB (11224981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe249b22d1208ab649e89964eb464001e17f0046b2315ed1796765c0cc3fb536`  
		Last Modified: Fri, 18 Dec 2020 20:48:21 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0859b9ffe60d4d391f275eaaaee4bfeec4235827ba9720e566e25919bdd78b47`  
		Last Modified: Fri, 18 Dec 2020 20:48:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8dee3e26b2f583ab6fc7986b3eb18002c692d2139828ed18e4b482dd5c3cc`  
		Last Modified: Fri, 18 Dec 2020 20:48:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae398357c5a6fa7478d4577d20aac0205696d66462739713cd1ea8707617014`  
		Last Modified: Wed, 30 Dec 2020 00:57:12 GMT  
		Size: 4.4 KB (4395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70c2997997e56dd60881222607bb3df425a84ab993077535a82dc3e8233b420`  
		Last Modified: Wed, 30 Dec 2020 00:57:12 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:71c9dc69c2dd8877097c3cc1270f69b79fff9bbf0f6eb1222edb2091afa1ca40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12988706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3133112f23d480ffcd52d1b384e7933486f56b7c092bc2d6dfbf7f6e42bd3fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:35:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:36:01 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:36:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 05:51:17 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 05:51:18 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 05:51:20 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Thu, 17 Dec 2020 05:54:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 05:54:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 05:54:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 05:54:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 05:54:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 05:54:22 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:03:27 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:03:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 01:03:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:03:33 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:03:35 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:03:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fd93cc6a1e39bdb8121ae35ee402c25416b317da7efd7e27a38a4af80710b7`  
		Last Modified: Thu, 17 Dec 2020 05:58:49 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fc827812b79452d91ced463793937316b84ae0d091f1be8f633999b998bf4b`  
		Last Modified: Thu, 17 Dec 2020 05:58:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea10504d464945d969b5e865f81d5ef2f6e0cd37f019b1f6de01226ad88dfd1`  
		Last Modified: Thu, 17 Dec 2020 06:00:38 GMT  
		Size: 10.6 MB (10567702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befb30cf111644a6dc454723cd51e58f1fa375500de83d6f9bb6e745c691ddee`  
		Last Modified: Thu, 17 Dec 2020 06:00:33 GMT  
		Size: 7.2 KB (7154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f4318bdfeb6a791185dafa2ddf3f96556b1b940bd4df30cd24544766f43fa`  
		Last Modified: Thu, 17 Dec 2020 06:00:34 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9604313df56a7d88d260ac60c9bda7b244a4bd9b9e1938c3d815daea8d138922`  
		Last Modified: Thu, 17 Dec 2020 06:00:33 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b950ceb1a6c80a1e1f6896c0919634db3a096bdf4fa49f0b942df7277dfc6d4b`  
		Last Modified: Wed, 30 Dec 2020 01:06:18 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ded3b2496e03d137569b640e4179296ed3db53f4522980379731d9fbf0b544`  
		Last Modified: Wed, 30 Dec 2020 01:06:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:93d8a27afa2a6c63bfed7d162c5dbb6b36987b58e3c8c4fc592bbf2e11c0eee7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27997dc924b5919ebaac7d9be741432c81aad77f8d76e622cedc65206d92d625`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:01:11 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 04:01:19 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 04:01:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 04:20:22 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 04:20:23 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 04:20:25 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Thu, 17 Dec 2020 04:22:52 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 04:22:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 04:23:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 04:23:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 04:23:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 04:23:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:45:34 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:45:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:45:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:45:49 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:45:55 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:45:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20223af9aac4511a0a9a78463ff758585620e621be0678319eba90176b7e615`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2482f57ac4ab8ff038d0589f0507eea54d56adf3da98ff95df25c6beb575c1e4`  
		Last Modified: Thu, 17 Dec 2020 04:28:04 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46d87c6b8167ffac1b89447901d049264255ebed26c7e544bb8b0c97ac0df1a`  
		Last Modified: Thu, 17 Dec 2020 04:29:57 GMT  
		Size: 11.5 MB (11518273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8952926e929de220a0d4daf8f607b7f7ac56bc0f4cf34ac929250dc061f42c5a`  
		Last Modified: Thu, 17 Dec 2020 04:29:51 GMT  
		Size: 7.2 KB (7163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00907a241881e56ce6afb9a41fcc6a72391843b3526902f3f1dadd742faa186b`  
		Last Modified: Thu, 17 Dec 2020 04:29:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db1106eb6ce25010a4ce79be3a5a132f5298530ebab86cefc3128759a3f179`  
		Last Modified: Thu, 17 Dec 2020 04:29:52 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c048d7d94646cacc5f2e0de0195544f087175a97f583107ca8d2f10683431d93`  
		Last Modified: Wed, 30 Dec 2020 00:48:42 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61cd284405de8263ace80bbf6c4f1b1f8334cc0d9522c7bd1adfcca7e7635c5`  
		Last Modified: Wed, 30 Dec 2020 00:48:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:3914c000740ee1540afe736d5c6b56194b91c3aa83cba76cfffd4e0f08d6bc62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15113683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91da971ba4bccbe72f56994255a99f273c81cf8b72f69e80611853f1e728b96f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:49:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 05:49:56 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 05:49:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 06:03:30 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 06:03:30 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 06:03:30 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Fri, 18 Dec 2020 20:50:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 20:50:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 20:50:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 20:50:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 20:50:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 20:50:17 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:41:56 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:41:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:41:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:41:58 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:41:58 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:41:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305178ae8cb85c448e0963870f5425a527c36dae59155568c8da341f4173b82`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3614159f507682c618782d96e8e35ed8b175b4dff44e39ef793184e39ba180`  
		Last Modified: Thu, 17 Dec 2020 06:07:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a33958ae23a3ee135349d61f8d01c38a05870913ce45d0c547cc8b75db7b3b1`  
		Last Modified: Fri, 18 Dec 2020 20:56:15 GMT  
		Size: 12.3 MB (12306231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e9195bb494783bdbdd0660882c11db048eb86877e2b1a25aecbb0f2f3f4ff4`  
		Last Modified: Fri, 18 Dec 2020 20:56:11 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf1c9bc2a6141b5757cb4fbcd71d18d39e2076fdb03eacd8ca366360053bd45`  
		Last Modified: Fri, 18 Dec 2020 20:56:09 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bb804d5d1d34a9c351b9f62eef3a38b45b496c9a1a9aa84b4617852db3e67b`  
		Last Modified: Fri, 18 Dec 2020 20:56:10 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677dd4b16a6ed6f020b89a1a82af28a6d42b0487b7e10658476be71d11e5b5a6`  
		Last Modified: Wed, 30 Dec 2020 00:43:35 GMT  
		Size: 4.4 KB (4392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed346e0aa19e0087b2c6757f9af2192c5d5ba6769d0394a654b830892fd773`  
		Last Modified: Wed, 30 Dec 2020 00:43:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:1ec6d0541da759e7bf35f562aeea0106092d1bc09312507cd0ada318e721fe34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15439028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9655e8da4ea7a50492d5225f880546088393e0092dc8b6cf4472a10a0380551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:27:05 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 08:27:07 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 08:27:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 08:47:26 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 08:47:32 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 08:47:36 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Thu, 17 Dec 2020 08:49:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Dec 2020 08:50:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Dec 2020 08:50:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Dec 2020 08:50:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Dec 2020 08:50:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Dec 2020 08:50:22 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 01:20:59 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 01:21:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 01:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 01:21:13 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 01:21:17 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 01:21:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9020dece47a455612905a0f9d5608b39b5cfa68bf304d4473bbbee3f085dce3e`  
		Last Modified: Thu, 17 Dec 2020 08:55:18 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd7a09fca54bf573268df0318667b22454de76b77537ce6968b9a9e3a5bd2b7`  
		Last Modified: Thu, 17 Dec 2020 08:55:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15893102c7418bd27c2c0082ad7742ae5d0e69b3242eed5bc81408cdabd8ab67`  
		Last Modified: Thu, 17 Dec 2020 08:57:11 GMT  
		Size: 12.6 MB (12620345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c3900046078572db0a950e71210da625a7948bb75e80b1b3bfe2a332761797`  
		Last Modified: Thu, 17 Dec 2020 08:57:04 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e05efdc5674bcc241ee4db4cc0ff9df2d70a09b11c74d5bef7816944d7846d`  
		Last Modified: Thu, 17 Dec 2020 08:57:04 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d78661e48176d17518ece3d2f6f0f1c83788bc0202f7a60b9d35c3b8e18af3`  
		Last Modified: Thu, 17 Dec 2020 08:57:04 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bf9a7b78f97aa3f29113fdf30dd615615cab62a8c6932ac5c2b9e18592b15b`  
		Last Modified: Wed, 30 Dec 2020 01:23:40 GMT  
		Size: 4.4 KB (4396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ce8672c12482dd61649c907abc75f28cf05c7938885bccb452dacf1c07ac2`  
		Last Modified: Wed, 30 Dec 2020 01:23:39 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:1f90ffd8e1ed90dc01970b8ce21c645a0617b693355f554ffa317e4f87a0c7f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14072210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe09f3107645b442a47010a74cc0cccd3934dcab0c6fc866605cbae547cb0db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:43:56 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Dec 2020 09:43:57 GMT
ENV LANG=en_US.utf8
# Thu, 17 Dec 2020 09:43:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Dec 2020 10:01:48 GMT
ENV PG_MAJOR=9.6
# Thu, 17 Dec 2020 10:01:49 GMT
ENV PG_VERSION=9.6.20
# Thu, 17 Dec 2020 10:01:50 GMT
ENV PG_SHA256=3d08cba409d45ab62d42b24431a0d55e7537bcd1db2d979f5f2eefe34d487bb6
# Fri, 18 Dec 2020 23:01:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 18 Dec 2020 23:01:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 18 Dec 2020 23:01:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Dec 2020 23:01:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Dec 2020 23:01:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Dec 2020 23:01:46 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Dec 2020 00:46:27 GMT
COPY file:d98720f44754747f666c604efdd82f7c897ce6bdbdfb328f1b7ffc977a4060b7 in /usr/local/bin/ 
# Wed, 30 Dec 2020 00:46:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 30 Dec 2020 00:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Dec 2020 00:46:30 GMT
STOPSIGNAL SIGINT
# Wed, 30 Dec 2020 00:46:30 GMT
EXPOSE 5432
# Wed, 30 Dec 2020 00:46:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec909f7d148e1f5c76f40f0fe4cec25c8a0f55dee05e382db0c692d59f7c084f`  
		Last Modified: Fri, 18 Dec 2020 23:05:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fadc63f7954f50d02abf819a5f8693cf92f86873d00c4dd5108f7dbbf5e0c48`  
		Last Modified: Fri, 18 Dec 2020 23:05:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5176239b5867b77edf4396755a17204392b966860718ec133488dac7729599`  
		Last Modified: Fri, 18 Dec 2020 23:07:21 GMT  
		Size: 11.5 MB (11491731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e3824f15275868bc5c9e66971a7fe3c24d29d1a2abf82840d52a54cbd7e343`  
		Last Modified: Fri, 18 Dec 2020 23:07:18 GMT  
		Size: 7.2 KB (7160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e411a35f99101ee655e0b393ff618781421d9847bbe8e9b39099011580a0545`  
		Last Modified: Fri, 18 Dec 2020 23:07:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63961fb349454d857ad0a65569bff82021db9aa9aa206260497bc8f0c76a7ac1`  
		Last Modified: Fri, 18 Dec 2020 23:07:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabfbae595b89fb552a2329bfcc2a8e3b1daa5267ae3d2b5f14892f172cd1acf`  
		Last Modified: Wed, 30 Dec 2020 00:48:28 GMT  
		Size: 4.4 KB (4393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b64a0e4cfa470808be18c02abad6087c16438dbc6b870c22f6f4fa151d0cbb2`  
		Last Modified: Wed, 30 Dec 2020 00:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
