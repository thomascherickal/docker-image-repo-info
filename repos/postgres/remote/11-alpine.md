## `postgres:11-alpine`

```console
$ docker pull postgres@sha256:604affc95d5070daab68d0060cd433b629f94c2d37db03f9b864bb304e6c8820
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

### `postgres:11-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:948764873f7fd951ef728bcd6877167a0ce48d53806de6b6ad0b66f5adc454a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80025063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b60b8672f7eaf636e5e7ce2a54596210f0206b6ef73ecb7477286785957b8a8`
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
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:52:40 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 00:52:40 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 20:00:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:00:36 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:00:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:00:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:00:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:00:38 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:00:38 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:00:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:00:38 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:00:38 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:00:38 GMT
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
	-	`sha256:cdc4cd50101a1eba216e0c769881bd872ff77912c37daf37ac707d1e316c7aa4`  
		Last Modified: Tue, 08 Mar 2022 20:11:14 GMT  
		Size: 77.2 MB (77192182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daccb30273e157cfbd848aba64390ebf22eb749e399778c17d4f4397e17d1e6d`  
		Last Modified: Tue, 08 Mar 2022 20:11:03 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07189b4b31bc2a0ef9527f9be81a67c45207ff737affdd9347032e7b0917a09c`  
		Last Modified: Tue, 08 Mar 2022 20:11:03 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6631a30932bae903b8d35fe78a54c14cc3510760ce34bfed092fa30b2e7625a6`  
		Last Modified: Tue, 08 Mar 2022 20:11:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d298d9ef9dae19d9028d86bf270874104f221c2b38f464697e5bc0f19a87000b`  
		Last Modified: Tue, 08 Mar 2022 20:11:03 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:8aa83cd27ad6ef5794d3a8a911b36346233b1920d0c6c4aa6fe943e0c5a7f356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76539335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f40a65c577982ef78040213c6b15a4a6d62e87c2ab05853e95a0b29afbec3f44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 09:33:37 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Mar 2022 09:33:37 GMT
ENV LANG=en_US.utf8
# Thu, 17 Mar 2022 09:33:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Mar 2022 09:50:00 GMT
ENV PG_MAJOR=11
# Thu, 17 Mar 2022 09:50:01 GMT
ENV PG_VERSION=11.15
# Thu, 17 Mar 2022 09:50:01 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Thu, 17 Mar 2022 09:54:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 17 Mar 2022 09:54:47 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 17 Mar 2022 09:54:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Mar 2022 09:54:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Mar 2022 09:54:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Mar 2022 09:54:51 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Mar 2022 09:54:52 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Thu, 17 Mar 2022 09:54:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 09:54:53 GMT
STOPSIGNAL SIGINT
# Thu, 17 Mar 2022 09:54:53 GMT
EXPOSE 5432
# Thu, 17 Mar 2022 09:54:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8357a39915fb976ee53735630d407cf3039a8804160e32ecd63d7206dd0e49`  
		Last Modified: Thu, 17 Mar 2022 10:00:50 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68a50d25506682f9d05b7bf766ef5cf0bddb6785e086d10c03f83e050fea12b`  
		Last Modified: Thu, 17 Mar 2022 10:00:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0901d0b3d43b8ca59eb9c55b77b2a6b4cfa73d6ac2df0ff22d9cb17ddbb608`  
		Last Modified: Thu, 17 Mar 2022 10:04:49 GMT  
		Size: 73.9 MB (73899889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e624343f4613f657aca7a37f1cf6beae1f58b1ab44e52760db623f1e2e509d8`  
		Last Modified: Thu, 17 Mar 2022 10:04:08 GMT  
		Size: 8.0 KB (7986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e33785e0009c5b4485efb1ae70cef8bd4dd8a0c3ff050b8e341bd7de6e06ba`  
		Last Modified: Thu, 17 Mar 2022 10:04:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fad37000402a8fa799be2b27f143e8fb649b9cbf8ee08474bee716d8b1b8e9a`  
		Last Modified: Thu, 17 Mar 2022 10:04:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822ade8d3154eea96f999056c0b3b05b32c994567f23f6d7b1301b0b5654c2ad`  
		Last Modified: Thu, 17 Mar 2022 10:04:08 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:81c60c572914770f814937974f1feed34ca7e4dd680bbbbfb72ae3bb04e14fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73177312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbaf891ca3ca7ea070d6acfc53160344d1e296fb6e2d42e3b0d40b71c9fac27a`
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
# Tue, 30 Nov 2021 10:00:55 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 01:59:14 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 01:59:14 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 23:08:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 23:08:23 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 23:08:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 23:08:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 23:08:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 23:08:27 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 23:08:27 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 23:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 23:08:28 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 23:08:29 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 23:08:29 GMT
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
	-	`sha256:966d5eb40f44ba35f0fba070455e3c1770f0a05afe7d6de8538c0c49b6f80828`  
		Last Modified: Wed, 09 Mar 2022 00:10:27 GMT  
		Size: 70.7 MB (70728074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e07029f6756d158ebf18b30e73857cf3da6e554aafa35a493ba2366b589e69f`  
		Last Modified: Wed, 09 Mar 2022 00:09:50 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a279d435162d564631f553b8ac16d3fcdddd9fe0ca461dabf7b8f16bdb6b4e`  
		Last Modified: Wed, 09 Mar 2022 00:09:50 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b647413f71bc067714145634afbbf0714faef7bab79e04b4b4e1ecbf4110659c`  
		Last Modified: Wed, 09 Mar 2022 00:09:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61984d531df3d06d43cecd4c0ce487842bfdf2bf5d0d8d1c687dc5da373a88e`  
		Last Modified: Wed, 09 Mar 2022 00:09:50 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:701ffe56af890fe5724fbbed2a9a2eac2f68a17eb6d13a81837ba046cc8e59e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78757297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb36413600e4326bb90fb008fd6bd798410d9b79c14de82e8a5b381c30ad887`
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
# Tue, 30 Nov 2021 04:50:33 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 01:11:46 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 01:11:47 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 20:21:20 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:21:21 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:21:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:21:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:21:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:21:25 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:21:27 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:21:28 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:21:29 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:21:30 GMT
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
	-	`sha256:53fead03fe0be36dc00f6924990ce99017aac3a27db2dc7627ed983f5dcf2fac`  
		Last Modified: Tue, 08 Mar 2022 20:39:59 GMT  
		Size: 76.0 MB (76027502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40c78ee265640893582e736777c08c1ed315b8d5b32875f66bc0dc1f738b9d7`  
		Last Modified: Tue, 08 Mar 2022 20:39:49 GMT  
		Size: 8.0 KB (7987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d35395fa4913f93e2332b3fd7d975ccb55fce6cecf8e0e53aee4543a336736`  
		Last Modified: Tue, 08 Mar 2022 20:39:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c831eca294bf17e7c7e83383ec338289d1143fae8353182bfb6ec7718b1f8`  
		Last Modified: Tue, 08 Mar 2022 20:39:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f73a3e23c4033e4bac8b9f5ea8c7fcfb36d90c4d2c4c5daddf58dc0c1db6e5`  
		Last Modified: Tue, 08 Mar 2022 20:39:49 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; 386

```console
$ docker pull postgres@sha256:8678811df9e23bdb156aeba8ba80cd579cd81a0ff1c166945b60d244f06ca3dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.8 MB (84751193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e916c3eb72e86f264a693a3a543a275744d3ba3ad671a94a9dcad5de88e01c7`
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
# Tue, 30 Nov 2021 03:58:37 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:26:41 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 00:26:41 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 21:02:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 21:02:29 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 21:02:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 21:02:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 21:02:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 21:02:30 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 21:02:30 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 21:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 21:02:31 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 21:02:31 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 21:02:31 GMT
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
	-	`sha256:ffec3cb0fdcf943cb0dfb84ad7be4cc9b82bde6e6bf037335eb7cde788c5b208`  
		Last Modified: Tue, 08 Mar 2022 21:22:43 GMT  
		Size: 81.9 MB (81909608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b96fe8c82e4bd7f53a7011837ed11515a2feacc2c5bb1e146792f1b12e2f11f`  
		Last Modified: Tue, 08 Mar 2022 21:22:29 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca08b6fb125779a51e593e1f450daf895ecf319155a9fb35f84311716265ebc`  
		Last Modified: Tue, 08 Mar 2022 21:22:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b5888a4af8499c2a3e1fe49ae77a19b1b03e11218e2de8ab7bd615c91982d1`  
		Last Modified: Tue, 08 Mar 2022 21:22:29 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a901e880f1a6c7a81fb4920ababebdbf879127046dcd1c5f2fe04f25a0f8c497`  
		Last Modified: Tue, 08 Mar 2022 21:22:29 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:171b40b4bd986a66045700be02fdc92891676b585446b81af525c9b6b6f4ee4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85133757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719c864c8a64f97cd7d3aec41a6be30378f6fe76431ed989fada34f42728632d`
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
# Tue, 30 Nov 2021 04:49:48 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:26:11 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 00:26:14 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 20:56:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:56:20 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:56:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:56:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:56:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:56:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:56:43 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:56:56 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:57:00 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:57:04 GMT
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
	-	`sha256:67e505ae19f18eb9689dd0a1df6c89ba3f5a77e024d34da986e734b68d1f74ba`  
		Last Modified: Tue, 08 Mar 2022 21:12:54 GMT  
		Size: 82.3 MB (82304504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f722ed5946f40e0c8b4df06a50a58688774bdedee3e3c37e6aedf7ba99d780`  
		Last Modified: Tue, 08 Mar 2022 21:12:39 GMT  
		Size: 8.0 KB (7989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c1f9892f6baf4bc205ef885bc794ea220ce3b1f5ec1c8c44b691302755d8f`  
		Last Modified: Tue, 08 Mar 2022 21:12:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660e8ea0371564654b9808bd8e1243fb3699bf4e5c0b6541de95c02a16971908`  
		Last Modified: Tue, 08 Mar 2022 21:12:39 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aad697ccfcc731a5b9f2009eea810db7f31c1ad36a7557015e11a35756785b`  
		Last Modified: Tue, 08 Mar 2022 21:12:39 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:3732a5e68ad8fc1c237cd2124dd7462eadf9522042b1aa4d6d7b13e6f5cc2c49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.9 MB (80912970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a207c69eee9288aea2d6876a17d4cb363e68f3fda9d3ff2789168f8393dfe3e`
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
# Tue, 30 Nov 2021 09:23:43 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:23:00 GMT
ENV PG_VERSION=11.15
# Sat, 12 Feb 2022 00:23:00 GMT
ENV PG_SHA256=c8f58e8ebd4f4567f4f9ba1032eb3e99e0251d87cbe3e564b485590e37a879e3
# Tue, 08 Mar 2022 20:33:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm-dev clang g++ 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		zstd 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-krb5 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Tue, 08 Mar 2022 20:33:47 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:33:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:33:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:33:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:33:48 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:33:49 GMT
COPY file:e8928645623137de410cce68a2aa3b22f07a64e6391025598a60f3e461c606a3 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:33:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:33:49 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:33:49 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:33:49 GMT
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
	-	`sha256:515f7b83542d07f931555b4b88ccc546b542c71af114a23195754f29b89236f8`  
		Last Modified: Tue, 08 Mar 2022 20:46:44 GMT  
		Size: 78.3 MB (78292549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04279528e8bdf805b779289b283627eab3f8579a87213b1869c7b70732d292e`  
		Last Modified: Tue, 08 Mar 2022 20:46:35 GMT  
		Size: 8.0 KB (7989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbed28f06d738a6a56c6720a119c75de74b974a54bdb073bd1b54beadf62e7`  
		Last Modified: Tue, 08 Mar 2022 20:46:35 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190d0e1194a6321e179e18c2eb8fc70a29edbc7584cd04020d934aaef2446b87`  
		Last Modified: Tue, 08 Mar 2022 20:46:35 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473cca443227b986af601b4136a66c1332b4e5ca0be9827b6bdb48b55b1f2cc3`  
		Last Modified: Tue, 08 Mar 2022 20:46:35 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
