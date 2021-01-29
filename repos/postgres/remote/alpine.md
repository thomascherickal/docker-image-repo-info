## `postgres:alpine`

```console
$ docker pull postgres@sha256:16af09e480c49226f8e7cd4d602ab27e59f434eb255d2b45bd0cfe1defb86fd7
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

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:e90025c179830bbdcb8b75bcb4531f860a8fdf183922526f90063034ae853094
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62260252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6053d81a45b455a79e7abbc5b4d8410735f060634d345f70b0530b1d50b2b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 02:53:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 02:53:55 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 02:53:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 02:53:56 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 02:53:56 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 02:53:56 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 03:01:17 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 03:01:18 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 03:01:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 03:01:20 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 03:01:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 03:01:21 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 03:01:21 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:01:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:01:22 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 03:01:22 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 03:01:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff5918c11c3ab1f2763192c7c033f5dfe60b30d369a8aa483d65326974b637a`  
		Last Modified: Fri, 29 Jan 2021 03:42:07 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c393806625cde0c68d6881aaeb6a8305d841ad1ec4e6152fe5dde27a6c7b4af8`  
		Last Modified: Fri, 29 Jan 2021 03:42:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9307f3bcca3a3c96fa4f21cc851f49f877096fc2626817d148d1c8cbc70bcb25`  
		Last Modified: Fri, 29 Jan 2021 03:42:20 GMT  
		Size: 59.4 MB (59434340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eee78b95230e292517369656c57174ab474a5816040c1c9b97857e2b1d151ef`  
		Last Modified: Fri, 29 Jan 2021 03:42:06 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f2174cad0ecea8b84d0f6fb84fdb82b77623253a01f65f0854bcb26be6c24a`  
		Last Modified: Fri, 29 Jan 2021 03:42:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6b4e21c9936b9d3a480bcc26a0b6e7a4fb71f11e70c63f4da7953d0c8dbc92`  
		Last Modified: Fri, 29 Jan 2021 03:42:06 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1011823211fa960c4dae9c5929e2b284c9617492e99ffbf7f95d91c709606401`  
		Last Modified: Fri, 29 Jan 2021 03:42:06 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:1327e656b2dd5e9fa8d3e8e41483087a34b3e0b22b3fd87b550064b60323a939
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.6 MB (60569944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:369272409ea98ad8f2565fc0c56f2a186021fbfa69f22a8f49d7e9b30e57d08c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:09:22 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:09:23 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:09:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:09:25 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 01:09:26 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 01:09:27 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 01:13:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:13:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:13:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:13:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:13:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:13:24 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:13:24 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:13:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:13:26 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:13:26 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:13:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47814bcbfb45802646b189af4a9bc3e4510a538b55fd2808df448ec5e6491cff`  
		Last Modified: Fri, 29 Jan 2021 01:32:14 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e4686dd674a32664773b275c120c9879a27454fb70c89ea4663315c3b84c6`  
		Last Modified: Fri, 29 Jan 2021 01:32:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8544364e69e45c088cec7741bfc86678755d220960ab6085971b208453a26cfc`  
		Last Modified: Fri, 29 Jan 2021 01:32:31 GMT  
		Size: 57.9 MB (57933463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ad69d370f66f30feaed5908dad55683bab9009ed30302b1b082b037f9ca16`  
		Last Modified: Fri, 29 Jan 2021 01:32:13 GMT  
		Size: 8.5 KB (8538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6df55a4a74ee31526168f7e238eea26498febfbfeb9a95fe4178f908c217c1`  
		Last Modified: Fri, 29 Jan 2021 01:32:12 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10b7a405b5c73b2e4c8f52b148319aceee7fd36328559dc9d4a69b5867709ce`  
		Last Modified: Fri, 29 Jan 2021 01:32:12 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a458cbd2996e049c7ee4ff8166771aeebc09817661ced95bb8f544f78451312`  
		Last Modified: Fri, 29 Jan 2021 01:32:12 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:b5093e1c8f7fe04664d48031e3035b6aa97969215e27205e2b5ed568221e28c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57603911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f4d87a476e215e505d4bdb2a1590b95375904e03e7757824334796b30be884d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:46:41 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:46:42 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:46:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:46:46 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 01:46:47 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 01:46:48 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 01:50:31 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:50:38 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:50:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:50:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:50:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:50:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:50:47 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:50:49 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:50:50 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:50:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fa668b3d0ed9168e26ae186f3e531d3ae1e280d94f950446b3683eaaab37c8`  
		Last Modified: Fri, 29 Jan 2021 02:09:19 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f921cd3d5ba006be49bcfc3c119ff3d8f5d35fbc011e764afbbce4ee5b61b4`  
		Last Modified: Fri, 29 Jan 2021 02:09:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328396e657d0e2aa67a5c6de7b8ec405378ead69588ec11f950a9dc8ef06d839`  
		Last Modified: Fri, 29 Jan 2021 02:09:32 GMT  
		Size: 55.2 MB (55165632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfefab200932a3ab408aa224e85e5ed060f2b548fb9fab1a399b67be05e7f2c2`  
		Last Modified: Fri, 29 Jan 2021 02:09:16 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7998519f45031204d3f283ddee9fe1276482b1270e376b7fc74a8752060bb241`  
		Last Modified: Fri, 29 Jan 2021 02:09:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f931cd32a9c6ac09b3f73fbcbc89c1263d1ad2cbe7c8e6e682e9b1c7569917cf`  
		Last Modified: Fri, 29 Jan 2021 02:09:16 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd9d9b26159ec1be9625c2928ba3a3fdeff846052d150a9d63b21dc83e6e3ba`  
		Last Modified: Fri, 29 Jan 2021 02:09:17 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:82d86de81e5d0ec17d3760845120c8eebaf866e95541e7edceb07269c52b36ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61529484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adbbd4ee7e101af7aaef601c7ec9fe4e6788c77f7a75fed158740b4ea19aeb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:52:23 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 00:52:24 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 00:52:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 00:52:27 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 00:52:28 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 00:52:29 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 00:56:02 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 00:56:06 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 00:56:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 00:56:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 00:56:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 00:56:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 00:56:14 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:56:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 00:56:17 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 00:56:18 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 00:56:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84190c434223807f9b123dbab6b871f4d978fc7fcfb7bd372aae021a3f90b9cf`  
		Last Modified: Fri, 29 Jan 2021 01:16:24 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23887416d5dd038d93a43a59a6bc616f68e5f6805f3aadcedb9577d2274a5f0`  
		Last Modified: Fri, 29 Jan 2021 01:16:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3ee89fd4549d7061710dd37514bc6cba800dc99f7a9c34d17d804ba1da6318`  
		Last Modified: Fri, 29 Jan 2021 01:16:40 GMT  
		Size: 58.8 MB (58803499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483e8077a101e2825ad338fdea34a1d7f706d95f31cd26e1243d575b6793b5c`  
		Last Modified: Fri, 29 Jan 2021 01:16:23 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd991b5229550224576632e819987a50ab81580d18765777daae2b07986049`  
		Last Modified: Fri, 29 Jan 2021 01:16:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22422c0a856b3f70d82bad08f96545ceda209baf070f54ef6fa6af499dceca3d`  
		Last Modified: Fri, 29 Jan 2021 01:16:23 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6092c2652248d5e9d574f5d04ee93638a20d8fccd85d9873366e1f31234cd28e`  
		Last Modified: Fri, 29 Jan 2021 01:16:23 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:0470abb31fe613f734992f443e38da517b61db9a79e987147853d071b1a5eb76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.8 MB (65842365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6366807589f882f13927465d8c7a13250ab1c432247135ac1aa0014e4e43025c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 03:03:57 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 03:03:58 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 03:03:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 03:04:00 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 03:04:00 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 03:04:01 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 03:17:09 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 03:17:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 03:17:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 03:17:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 03:17:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 03:17:15 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 03:17:15 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:17:16 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 03:17:17 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 03:17:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6577fee13210fe1c3f4549f1ef86d700f99fac79b2fdd5b840c7e298d9ff5899`  
		Last Modified: Fri, 29 Jan 2021 03:55:44 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4cc8bff7850ed45d5f7c08b1b4f9325ba2867fd9e91d3cbfa84e30234509ce`  
		Last Modified: Fri, 29 Jan 2021 03:55:44 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59fb48f0995a9b096ddc6449d496afbd206e5a393903d62055a02335d910323`  
		Last Modified: Fri, 29 Jan 2021 03:55:59 GMT  
		Size: 63.0 MB (63010148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a9a60a6e47a6ea1a264e673bea0b3b1e6ff5ee8d58667993266dbe22ed4af`  
		Last Modified: Fri, 29 Jan 2021 03:55:43 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a350c4e9e55e8e925da9b917d78f00857477f6f4193217dc64792e46e1a59`  
		Last Modified: Fri, 29 Jan 2021 03:55:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3710a9c90e6273f25ed365714c6247c2357e188adc316ddca2c1c979145925f9`  
		Last Modified: Fri, 29 Jan 2021 03:55:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f15e89a141a6e2d35bb735e7e228b1017886d1ce56ede6665c6053a8c8b88c6`  
		Last Modified: Fri, 29 Jan 2021 03:55:43 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:f824154279d87aeccbf0a9ae6b8ec084b27d10dbff79f94fb565e8f59f097445
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64688974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02963582d402286f3393c3feca3b990aedc359c7f5ef53f66be130e4a9970fde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:48:47 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:48:55 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:49:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:49:14 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 01:49:21 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 01:49:24 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 01:53:50 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:54:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:54:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:54:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:54:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:55:02 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:55:05 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:55:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:55:21 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:55:27 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:55:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff06bd42b80b365bb0c19fbbbe316a95812c98b5963e0930ea89cc0c684a2833`  
		Last Modified: Fri, 29 Jan 2021 02:26:17 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf320aafe224f5aad678f29f514b47d6d4aefcd42e80b7041098c1da820f8c23`  
		Last Modified: Fri, 29 Jan 2021 02:26:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9888fa6f6eb392f5f094f7053ec93174edcab7b5e65dda420ee5cdf5d603d61c`  
		Last Modified: Fri, 29 Jan 2021 02:26:24 GMT  
		Size: 61.9 MB (61861727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bef199871ad981783234066c45d82c7ec48dec0ca9fd3303981f65fad72d3c5`  
		Last Modified: Fri, 29 Jan 2021 02:26:11 GMT  
		Size: 8.5 KB (8534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2652bd8d9dc227815234ab9a2e1a8e6073cdcc9284cf415b644cf6094f74b735`  
		Last Modified: Fri, 29 Jan 2021 02:26:11 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d232f80be578e4cfdf1fb3901cd3ddaed6c83fe26c899f43df7c9005e7825b81`  
		Last Modified: Fri, 29 Jan 2021 02:26:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d5cbdceaaf03912db2f04e242ac8cf16733bee55f14f53e91acdb74ebd4989`  
		Last Modified: Fri, 29 Jan 2021 02:26:14 GMT  
		Size: 4.4 KB (4408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:139162289cd17be74c9620b4a38c57227d0f7ea0832119c4b0fc05f67cb6827b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65015439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b1956eb014364b70b0b8007b1b9b576ffb008871a21bb2c1a40406242c7ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:28:50 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 29 Jan 2021 01:28:50 GMT
ENV LANG=en_US.utf8
# Fri, 29 Jan 2021 01:28:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 29 Jan 2021 01:28:52 GMT
ENV PG_MAJOR=13
# Fri, 29 Jan 2021 01:28:53 GMT
ENV PG_VERSION=13.1
# Fri, 29 Jan 2021 01:28:53 GMT
ENV PG_SHA256=12345c83b89aa29808568977f5200d6da00f88a035517f925293355432ffe61f
# Fri, 29 Jan 2021 01:33:03 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Fri, 29 Jan 2021 01:33:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Fri, 29 Jan 2021 01:33:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 29 Jan 2021 01:33:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 29 Jan 2021 01:33:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 29 Jan 2021 01:33:14 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 29 Jan 2021 01:33:14 GMT
COPY file:ad28506adc606e446eefc263bc99d4cb809e608d4f550956143bf13c82c91f85 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:33:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 01:33:15 GMT
STOPSIGNAL SIGINT
# Fri, 29 Jan 2021 01:33:15 GMT
EXPOSE 5432
# Fri, 29 Jan 2021 01:33:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb7987d6a49388c77e555f2547e538d557a90c40b705e0fe10a7ef952d82326`  
		Last Modified: Fri, 29 Jan 2021 01:50:33 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d07431bbbdfa6c1540603fded3d65695c350f29a3aa77a1e475296db695a5a`  
		Last Modified: Fri, 29 Jan 2021 01:50:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7f507ceaa7468b1da7ece1dd3edb98dc4da76e8c12d3784de8d83bb4a2051`  
		Last Modified: Fri, 29 Jan 2021 01:50:39 GMT  
		Size: 62.4 MB (62398657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af5c4cbef8a0b0d7982ffd9ab0a4bb0dfe3adddc235d5afdc0f75b24d1a097c`  
		Last Modified: Fri, 29 Jan 2021 01:50:31 GMT  
		Size: 8.5 KB (8536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb363f2ac79aefa9854f3b3a07efbad95ab3fae789551f5e3eea021857e095d3`  
		Last Modified: Fri, 29 Jan 2021 01:50:31 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8510cc57b56bdf7b62a20676c657ea773a87d5cc758678aca3d9e0cfe32a54e`  
		Last Modified: Fri, 29 Jan 2021 01:50:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f143b11d2ca10a1a5ec2385131728751a2313e4cbbd9df9b52880cc2e14e8`  
		Last Modified: Fri, 29 Jan 2021 01:50:31 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
