## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:a2c27b49aabbae8ddedb233ba8652adef19adfd8219dea2d8ded3d7650bc9732
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
$ docker pull postgres@sha256:f578cb63b548834c271316d10ca02addc2bd62cb0b9c39ea871a40819b4ba1dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14546597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371edead63487bc8cf899bbf3c1d364719bf9751ce92c9c570891e18890eaef2`
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
# Fri, 26 Mar 2021 01:38:26 GMT
ENV PG_MAJOR=9.6
# Fri, 26 Mar 2021 01:38:26 GMT
ENV PG_VERSION=9.6.21
# Fri, 26 Mar 2021 01:38:27 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Fri, 26 Mar 2021 01:42:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 01:42:30 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 01:42:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 01:42:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 01:42:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 01:42:34 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 01:42:34 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 26 Mar 2021 01:42:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 01:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 01:42:36 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 01:42:36 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 01:42:36 GMT
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
	-	`sha256:b1c8d5314c1a8d0f2ac87bf8e285318acf6e2a67910086a2ed0bbb7f045776ea`  
		Last Modified: Fri, 26 Mar 2021 01:49:20 GMT  
		Size: 11.7 MB (11721446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f92fadea6b573bc5f709db362cd8a31cfec0f1ce6b11ffbcee4e213b7ced60`  
		Last Modified: Fri, 26 Mar 2021 01:49:15 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cfe0be6d5a0742204affcbfc0665f0e4bd7d1c3882ebf28aba2cfd366def0a`  
		Last Modified: Fri, 26 Mar 2021 01:49:14 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d26ddff2efe180678f3f839ca09e32b12798d2a02ed738007fcd4586cbe95e`  
		Last Modified: Fri, 26 Mar 2021 01:49:15 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4103242e69beb654bd5a3f66950496426f699e44a9bd31d999b55827e22b1a8d`  
		Last Modified: Fri, 26 Mar 2021 01:49:14 GMT  
		Size: 4.4 KB (4409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f238f438765f82bab354c47eda0ab9997c654aedd3b53b69823e05c23097d`  
		Last Modified: Fri, 26 Mar 2021 01:49:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:5efaaa54820db32fce08500ff7f568909d97b1d47fc1c6a5c61f0c792c88a304
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13930624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da7ec0d923c83920de5c0aef9ab420a21e244c292df1f44db1f5d462bc328b9`
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
# Thu, 01 Apr 2021 00:33:34 GMT
ENV PG_MAJOR=9.6
# Thu, 01 Apr 2021 00:33:38 GMT
ENV PG_VERSION=9.6.21
# Thu, 01 Apr 2021 00:33:40 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Thu, 01 Apr 2021 00:36:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 01 Apr 2021 00:36:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 01 Apr 2021 00:36:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 01 Apr 2021 00:36:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 01 Apr 2021 00:36:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 01 Apr 2021 00:36:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 01 Apr 2021 00:36:33 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Thu, 01 Apr 2021 00:36:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 01 Apr 2021 00:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 00:36:39 GMT
STOPSIGNAL SIGINT
# Thu, 01 Apr 2021 00:36:40 GMT
EXPOSE 5432
# Thu, 01 Apr 2021 00:36:41 GMT
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
	-	`sha256:3f263225ed638d1d9dc69a297507da19a7e7b70b93fb1521f8ed1a34511a669b`  
		Last Modified: Thu, 01 Apr 2021 00:44:42 GMT  
		Size: 11.3 MB (11295043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe0f117ecc8dc00b80c9536531342d53251d80bc7712d966341811a9a8a921e`  
		Last Modified: Thu, 01 Apr 2021 00:44:36 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1160855696385372dbf6eb521168d46a5de329c889a2e02398635a89774416b4`  
		Last Modified: Thu, 01 Apr 2021 00:44:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c373a644d6cb82beb976e9f83cd83498f24eeb5441976a861b64e66b05474b3`  
		Last Modified: Thu, 01 Apr 2021 00:44:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6033964d5ab038e11a5800fc2340cc3743fff6e6350625ff38e6631a377c845a`  
		Last Modified: Thu, 01 Apr 2021 00:44:36 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9178d093c1f514c82387ede51198202b7709e3a9e1b2e0ba907080def00f83e6`  
		Last Modified: Thu, 01 Apr 2021 00:44:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5114e696f7d81bc6fc1f232eee2921e9bd2fe696407a4593ff6d24fb19d2a8f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13078743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d5ed734d7a49f0b7139cfe67f8839d0d5e4900211e780298d2889cf863dfe5`
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
# Fri, 26 Mar 2021 02:13:40 GMT
ENV PG_MAJOR=9.6
# Fri, 26 Mar 2021 02:13:41 GMT
ENV PG_VERSION=9.6.21
# Fri, 26 Mar 2021 02:13:42 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Fri, 26 Mar 2021 02:16:06 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 02:16:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 02:16:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 02:16:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 02:16:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 02:16:19 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 02:16:20 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 26 Mar 2021 02:16:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 02:16:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 02:16:25 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 02:16:26 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 02:16:27 GMT
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
	-	`sha256:00509102607260544b6eccfb577b432052561a8445b98d065f0dc6c4cab43a3b`  
		Last Modified: Fri, 26 Mar 2021 02:23:12 GMT  
		Size: 10.6 MB (10641274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c974097f2da281d2ecbf8d6a1110188d575a51e6d07c7d0ccf92f9587dbc52`  
		Last Modified: Fri, 26 Mar 2021 02:23:07 GMT  
		Size: 7.2 KB (7160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febce2333713cfa359c26dc1edeef3b0055cc5d676d09681d3fb6bff062ce384`  
		Last Modified: Fri, 26 Mar 2021 02:23:07 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b915a5b70fbb0c00e921c4c8fc9eb2bea271e4304c1032e93f014911333fe1`  
		Last Modified: Fri, 26 Mar 2021 02:23:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71661c44e5bd9774a208bba28d8615713f41bb357c528d65837a1fe8427591`  
		Last Modified: Fri, 26 Mar 2021 02:23:11 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0556822a3f5eb26e60bf8282bc8f0b9c6fffb604a48440657ae7e32d76bed80`  
		Last Modified: Fri, 26 Mar 2021 02:23:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:ec92e29d07c5664eb62e8c2cc002b2ba6f93a4dcb24c27ccf57af7fe1635fe16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14259939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8abe0ae9d9079e591bf5087c137f9d2c0d8ed8c92bb94a6ac21340bfc73d45ef`
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
# Fri, 26 Mar 2021 06:08:03 GMT
ENV PG_MAJOR=9.6
# Fri, 26 Mar 2021 06:08:04 GMT
ENV PG_VERSION=9.6.21
# Fri, 26 Mar 2021 06:08:06 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Fri, 26 Mar 2021 06:11:30 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 06:11:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 06:11:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 06:11:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 06:11:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 06:11:45 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 06:11:46 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 26 Mar 2021 06:11:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 06:11:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 06:11:51 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 06:11:52 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 06:11:54 GMT
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
	-	`sha256:0dcfab7631ddd6cca340ea3ecde9403bbe93aeb2878f04be04beb7d6266e9577`  
		Last Modified: Fri, 26 Mar 2021 06:17:28 GMT  
		Size: 11.5 MB (11534571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2001eb720fcdf34ca2497637a1dafcbdc7429723c11350ee8b37417d7b13e8`  
		Last Modified: Fri, 26 Mar 2021 06:17:18 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404236adfea7695c77a0c5dbcecd8c34bf996eb9e232de6829cb08230dc31524`  
		Last Modified: Fri, 26 Mar 2021 06:17:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8072f316c5d45ae50417ceec32e77b120b76a6717e114eb75471bf76ec7e`  
		Last Modified: Fri, 26 Mar 2021 06:17:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71beb989ada5e313301311ceed163436e11b222a9d5177813df6ab1e64cb145c`  
		Last Modified: Fri, 26 Mar 2021 06:17:18 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35c8b2e1b1d625408a7af32e820cac3ebb74f9ef8d180ad0fed6425d4d0d61a`  
		Last Modified: Fri, 26 Mar 2021 06:17:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:8e2f3c24c6343274fb9a5fd54c578799e1a62afbde747fcdba340f175065229d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15188006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598e717ef89ff493ce5b829b6009553c3f24fafcdb63567c049e8768ea87d7c2`
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
# Fri, 26 Mar 2021 11:16:21 GMT
ENV PG_MAJOR=9.6
# Fri, 26 Mar 2021 11:16:22 GMT
ENV PG_VERSION=9.6.21
# Fri, 26 Mar 2021 11:16:22 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Fri, 26 Mar 2021 11:19:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 11:19:45 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 11:19:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 11:19:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 11:19:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 11:19:47 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 11:19:48 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:19:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:19:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:19:49 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 11:19:49 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 11:19:50 GMT
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
	-	`sha256:f9e04ad13c4159211f7169e2749923463440e52537871b28b2b140a9506c7608`  
		Last Modified: Fri, 26 Mar 2021 11:26:56 GMT  
		Size: 12.4 MB (12356419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36e3de3c33e54febdc723b4faa7e9f91db343f9d384c1b09330af4d16b2720e`  
		Last Modified: Fri, 26 Mar 2021 11:26:52 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdc5ea4f943f54e437f6bf0cb686787202d09f210ec884bdd80c9551c705585`  
		Last Modified: Fri, 26 Mar 2021 11:26:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45062aa5297e33c38cbdf0925c03bc70aa950e27d7609c43c6c93d1b4fd69cd7`  
		Last Modified: Fri, 26 Mar 2021 11:26:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d943cc16da6deeab74f30f93ae7ebe80c20f439a4ec4dab17f4aefe2bf20ce`  
		Last Modified: Fri, 26 Mar 2021 11:26:52 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692b3fb54060232bf1a2d6f758a59a4762ade2f6834cc0186a6bff3fd501f01b`  
		Last Modified: Fri, 26 Mar 2021 11:26:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:13680072430d65132b48597c690fd0a9547e48871ad29cde14f187c65f8074d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15558532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc4755aa772d8a4860951de912fe3d58460401b5c5c1009851c2c837d9c7030`
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
# Fri, 26 Mar 2021 02:11:24 GMT
ENV PG_MAJOR=9.6
# Fri, 26 Mar 2021 02:11:33 GMT
ENV PG_VERSION=9.6.21
# Fri, 26 Mar 2021 02:11:37 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Fri, 26 Mar 2021 02:14:32 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 26 Mar 2021 02:14:50 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 26 Mar 2021 02:15:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 26 Mar 2021 02:15:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 26 Mar 2021 02:15:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 26 Mar 2021 02:15:32 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 26 Mar 2021 02:15:33 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Fri, 26 Mar 2021 02:15:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 02:15:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 02:16:05 GMT
STOPSIGNAL SIGINT
# Fri, 26 Mar 2021 02:16:10 GMT
EXPOSE 5432
# Fri, 26 Mar 2021 02:16:13 GMT
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
	-	`sha256:a94aafef1c0ad92d6403d96ad4d65906ec2da71d7d24ba55743e9140b2500911`  
		Last Modified: Fri, 26 Mar 2021 02:24:55 GMT  
		Size: 12.7 MB (12731944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42329b6b97d809a2a1d2ba1c5ff3b03ab5801b1dd2a15eb1f47a216242ad731`  
		Last Modified: Fri, 26 Mar 2021 02:24:48 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb67e3b0374340c65e00a20523062724a474561a89dcd1241694355e684c452`  
		Last Modified: Fri, 26 Mar 2021 02:24:48 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db142a93bd6508b5a5d4ba01a420228b56da3493d3c8ecd9f22a74e1927cd92`  
		Last Modified: Fri, 26 Mar 2021 02:24:49 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb29b7241e3926705976d6922c9274cd6a91e3415487f473d9c454ea940e6195`  
		Last Modified: Fri, 26 Mar 2021 02:24:50 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b65452ae54cdfd4fe6d7629b511492ea470a4bfbe73cee04b865faa7b106863`  
		Last Modified: Fri, 26 Mar 2021 02:24:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:7b19760767ecac8d9e625e3644e32ebbbcf1c722cddedfac607b0df07d3d278c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14224330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bcd5b4fd1e71cc1540409e425c03532b5914296f9d6856490b22fd7a506ec9`
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
# Thu, 01 Apr 2021 02:45:56 GMT
ENV PG_MAJOR=9.6
# Thu, 01 Apr 2021 02:45:56 GMT
ENV PG_VERSION=9.6.21
# Thu, 01 Apr 2021 02:45:56 GMT
ENV PG_SHA256=930feaef28885c97ec40c26ab6221903751eeb625de92b22602706d7d47d1634
# Thu, 01 Apr 2021 02:47:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 01 Apr 2021 02:48:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 01 Apr 2021 02:48:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 01 Apr 2021 02:48:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 01 Apr 2021 02:48:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 01 Apr 2021 02:48:02 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 01 Apr 2021 02:48:02 GMT
COPY file:e881105b30bb0f1591c0f7f6dfe19bf5351d029d5babae597d2698e04a16ec8b in /usr/local/bin/ 
# Thu, 01 Apr 2021 02:48:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 01 Apr 2021 02:48:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 02:48:04 GMT
STOPSIGNAL SIGINT
# Thu, 01 Apr 2021 02:48:04 GMT
EXPOSE 5432
# Thu, 01 Apr 2021 02:48:05 GMT
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
	-	`sha256:c23643ed91590b4bb8cf46f1e436e6977063925dc3a1f8496343b78edf985fea`  
		Last Modified: Thu, 01 Apr 2021 02:52:00 GMT  
		Size: 11.6 MB (11608267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62d246aa7cbbfb5178600db713a78b7d06d6def2c2a0cde9e56311769da4c4d`  
		Last Modified: Thu, 01 Apr 2021 02:51:58 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbbb7207ee570253b9f908a9cd4fce00a57d076f0b9191a43abe43446f0d5b3`  
		Last Modified: Thu, 01 Apr 2021 02:51:57 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d70cb224282452af36c664022bc8ca304476bfda8183e7b1fae18c1446c4e7`  
		Last Modified: Thu, 01 Apr 2021 02:51:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb5256f196a44377f3e325c524d5ac22ace6769455e8c6312bf3d639b581133`  
		Last Modified: Thu, 01 Apr 2021 02:51:58 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286459d7e3bc922f431313379c54de7c653f5e5e3fa08662ac11329297a5d011`  
		Last Modified: Thu, 01 Apr 2021 02:51:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
