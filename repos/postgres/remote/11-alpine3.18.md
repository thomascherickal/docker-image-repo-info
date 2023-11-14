## `postgres:11-alpine3.18`

```console
$ docker pull postgres@sha256:adbfa9043a9c702cc77309d6bd0edb309d6b70c14929e9e8f1f87caf36e99bbb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `postgres:11-alpine3.18` - linux; amd64

```console
$ docker pull postgres@sha256:54318123a11b0d7e5732f3cf10d1a5c508723983e2e0e25a4a76d33f6d210b2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91855189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16a569f28a97631e8d816666c9d08e65af7bf5e3e9f6902f33c94ad99ee6c0f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3043a3a9a263b4776de321cfb5c3d1244adec7976bd8de1714a88040446b2ff`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:744caea5f20914074549d4a340756588918ba5c0c2a456b51bf24f13e0a61d43`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:992bfbe780e1fb6d18ee35ca11c23686623f5f350037d0290a55d7582fb38172`  
		Last Modified: Tue, 14 Nov 2023 01:24:40 GMT  
		Size: 88.4 MB (88438779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5927836cf400021ef8936155a85dcc88107c94c321e394c75ff27563f4e65d9f`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 8.0 KB (7982 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aea2281ec2070cd35198a21bcfd148fa7de4f340c50ce83053a62f540dcc7be4`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27a994fd4f6a62d539c768c1173829b02de632dead9423feaa272f6b8dbbb2d1`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:184a4129e763ed0c2656956f3f5575434d8cbcc2f8e30422becb5a17cb4f7905`  
		Last Modified: Tue, 14 Nov 2023 01:24:38 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:595d0995d640744d9541fb17b0c9398437c68cf210b5d180ad8ba48bde45f1b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.9 KB (841857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9919d16403efa91a8b78b28db6a8a314dbc160e7e9354c79d4f10d33a272c554`

```dockerfile
```

-	Layers:
	-	`sha256:07966f7f6ef9c680797f71eccf1632b2cc072d16f1f833ae07efe9057d165428`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 806.1 KB (806140 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:65ac04b5948152f2b1ab3350266f8d1a7a333fa00d520842e1321e3ee5758708`  
		Last Modified: Tue, 14 Nov 2023 01:24:37 GMT  
		Size: 35.7 KB (35717 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:cfa8bcae7a9c6581ebc48a8d6d864279ead1becd530ded7412b4e10737f4c322
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90329973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca14e1171639ef84ffb9e0a40b6d2aa2c9af31b3a9b00af82dfbb2eb524c352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d85e8a1148e7602b0b44182dc8fa4c488db0b2e5ecd52e50022dbc19307fcf3`  
		Last Modified: Tue, 14 Nov 2023 01:25:29 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1e0d941bbfc194bc696cd55fc73d21834b0b4f8b19dae1baec3f8ce2550f11`  
		Last Modified: Tue, 14 Nov 2023 01:25:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612717b5b5ab8848607c6e116b314b5bd5bc4d1f28f68081da47380a8fb5473`  
		Last Modified: Tue, 14 Nov 2023 03:05:03 GMT  
		Size: 87.2 MB (87170236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c3e9b75457369a53a3a904b1ab4653fff9816b032ecc05979f6b3752446d2`  
		Last Modified: Tue, 14 Nov 2023 03:04:50 GMT  
		Size: 8.0 KB (7984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5db892258d8a7312a67710037304ce0a38c9f0604e21433384d59f26306feb9`  
		Last Modified: Tue, 14 Nov 2023 03:04:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb41fc719f81dd06cea76bce24b7ec192904615ce764a5aa11443a59dc9125`  
		Last Modified: Tue, 14 Nov 2023 03:04:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d15778c10ec45e2d2654a24d7331602f930703f22a0cb1ccce0773b05a64c0`  
		Last Modified: Tue, 14 Nov 2023 03:04:50 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d9a80011a1e2ce585163f1ed1f951d201e3f1d1ae4ae36e70dd3ffd9e380e26f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (84972259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fde69b1e2961cb67dfb9dcbcc7638abc60af55af140c35febaf0f7efa4b66f72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3de34561774cc0a52beeb06fef6a1f6af2bd2a08d4ea304d8d6da8fca56b666f`  
		Last Modified: Fri, 29 Sep 2023 17:52:13 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f40d1b3c22c63e3341b41845b4002cf47594b6e022558becb3c12725dbea465`  
		Last Modified: Fri, 29 Sep 2023 17:52:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b63fe9ff397c0142f6d9b2884bf3e002e70747c5624833900968ba03ac6d76c`  
		Last Modified: Tue, 14 Nov 2023 05:36:13 GMT  
		Size: 82.1 MB (82057911 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74c7ec7ec1b00acc3a347beb23b6e9904ae83c49770b53d1e81f8ba89aadf961`  
		Last Modified: Tue, 14 Nov 2023 05:36:10 GMT  
		Size: 8.0 KB (7983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa570103c05238ec90355acb34afbc81458fcb59888a37c5252aea09cbfec028`  
		Last Modified: Tue, 14 Nov 2023 05:36:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46715314d4fd4be725183f5f88541a2aa806ef0224d583474bd5421d00cb1200`  
		Last Modified: Tue, 14 Nov 2023 05:36:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:489b7bfacd2364700e386e7e6b2494de74a7ad026768fa34e901906b59dab9cc`  
		Last Modified: Tue, 14 Nov 2023 05:36:11 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:c4b6f6ac6f5a9862d8cea5b98be7a6f26fd544f9cceda5b7cac347ed09695f43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.9 KB (841862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c37aa34e711f97140b52a287c91ee3c832e7d4e492c6416c8e7d588fa9c8cb`

```dockerfile
```

-	Layers:
	-	`sha256:a7fe305f3ae6c042f376e8c58126d3d67670d1ef3224905a5e9da7e98da9c859`  
		Last Modified: Tue, 14 Nov 2023 05:36:10 GMT  
		Size: 806.2 KB (806176 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:556f03fd7b1b0d8c2379dcc43fffc2971c0f037380f9f9585b6abd0e1340b0cb`  
		Last Modified: Tue, 14 Nov 2023 05:36:09 GMT  
		Size: 35.7 KB (35686 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4d5459ab4a44c1e569d53ed6a86b5be97a583ec8287a541674cb7147679759e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90787592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23cf93d999d36e593caf6280fe1741705fb2664ea938432f49257ddf344c64a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:57128d869f4112bd058a44bc2fd19d9b05ea0895b34ad51c07e45ddadd30d480`  
		Last Modified: Fri, 29 Sep 2023 17:14:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1755e5b66878a2e0b911de75610a642179f0862fd67d7ac96105919310c7ee6`  
		Last Modified: Fri, 29 Sep 2023 17:14:32 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd306ee94945a9af063629090c51e7ed1120cbd25ea0748cd546bca37958a7af`  
		Last Modified: Tue, 14 Nov 2023 02:30:37 GMT  
		Size: 87.4 MB (87441323 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96d6bded8cfd7430b578b7644e17137711146a998c22e0c3cac2f485ed156b16`  
		Last Modified: Tue, 14 Nov 2023 02:30:34 GMT  
		Size: 8.0 KB (7983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aeec35d92b940ba51d3c3d3d440a9698539aedfbc34ec6242481c9991fd828c6`  
		Last Modified: Tue, 14 Nov 2023 02:30:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aec7e052edc99cb8608bcc8d7b91b345b7b0f7ca887d4a4921b4dc0b011f41ba`  
		Last Modified: Tue, 14 Nov 2023 02:30:34 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d941e56a535def27e343c1cdb5b2ca516eec2e651d3733beca5063219be34585`  
		Last Modified: Tue, 14 Nov 2023 02:30:35 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:058d8fd80cd2294223943d16dfd73c9c69bcad6481dd148602f1b68b468e2dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.7 KB (841712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6a17f8569c25b83afb7968af4b5b5b345a46e3448b8683f050962c5977e0765`

```dockerfile
```

-	Layers:
	-	`sha256:bc152fd9e931c11d5e00946691795bf9f725bcda72f40c753082d00e228b5548`  
		Last Modified: Tue, 14 Nov 2023 02:30:34 GMT  
		Size: 806.2 KB (806151 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9adc51596da5db8d6c9b4c26badf4117f5c60108ae9cc6d266747a6ae952fd6f`  
		Last Modified: Tue, 14 Nov 2023 02:30:34 GMT  
		Size: 35.6 KB (35561 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-alpine3.18` - linux; 386

```console
$ docker pull postgres@sha256:0c375b99378a06e845f9bb1a31c30a4e1e9012635c18a4bd2646544a12f4bada
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94599132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70de22b4395baf8aed25682a8bd93706e260a13fea15b791ad984d98555cec62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV LANG=en_US.utf8
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_MAJOR=11
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_VERSION=11.21
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_SHA256=07b0837471d5dd77b25166b34718f3ba10816b6ad61e691e6fc547cf3fcff850
# Wed, 04 Oct 2023 14:54:45 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.21","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.21?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 04 Oct 2023 14:54:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 04 Oct 2023 14:54:45 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 14:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Oct 2023 14:54:45 GMT
STOPSIGNAL SIGINT
# Wed, 04 Oct 2023 14:54:45 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 04 Oct 2023 14:54:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b13e500655c3825b1dc6c34be017288e52d1000e0645284425df9579d6a7da0`  
		Last Modified: Tue, 17 Oct 2023 19:05:35 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf4081add68802091c6e16b48534e5fe87ff7a4ec27801243c6b7f8315dc9c65`  
		Last Modified: Tue, 17 Oct 2023 19:05:35 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b635757f34cb3382aec556e52d4c2f700813909f83825520da63bbdd33f66a84`  
		Last Modified: Tue, 17 Oct 2023 19:05:40 GMT  
		Size: 91.3 MB (91348926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90cc0f8dec8defed210cbce73428edb18876f43a46356a7576d17f0d4c0675de`  
		Last Modified: Tue, 17 Oct 2023 19:05:35 GMT  
		Size: 8.0 KB (7987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45d9074f632e5552f352817fac358e7c54206f7fa917912b98605ce1a669b099`  
		Last Modified: Tue, 17 Oct 2023 19:05:34 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0a937045b7db8d22d91233136b94cfe8db300f1492e5db8bcad97f0f932137e`  
		Last Modified: Tue, 17 Oct 2023 19:05:34 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52022200f4e2fe3f9978657deaee56367b70a0defe627ed3f05f4efa23cbbda1`  
		Last Modified: Tue, 17 Oct 2023 19:05:36 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:1a0c50565fb0d704082ed891acb2f260918451b14fd9ae9de417afb8fb303fd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6ded4d0ec4c1020468178037bdb931129e3474d5476a414bfbe7348e9ebf5a`

```dockerfile
```

-	Layers:
	-	`sha256:3ad6f9653a43225f1a3d2d7adfcb838e8588469dd6ca4eefca0e73f7980de42d`  
		Last Modified: Tue, 17 Oct 2023 19:05:35 GMT  
		Size: 35.5 KB (35463 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-alpine3.18` - linux; ppc64le

```console
$ docker pull postgres@sha256:e1477676575a6778e5ad58332e1647a793c055850e103aa73edaf1cef28ff337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97216780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54e1d3823d5d2613cd6a055762b2694d2ce5873946b13d6285c6294b56136685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb0eda61a2703e25325ea1e358d3a74fe87529df79e6beb419567f1bdbbb63df`  
		Last Modified: Fri, 29 Sep 2023 17:20:30 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9b29b4ecd4028475762890da3e105d2ad2bb7690a0bff52c89c3d7180aca779`  
		Last Modified: Fri, 29 Sep 2023 17:20:30 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9fe1c00b26560a2277e4bc01644d6ed332584829e1092e8c66f0c2b923e71fb`  
		Last Modified: Tue, 14 Nov 2023 02:56:05 GMT  
		Size: 93.9 MB (93855828 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d16d2f6fb61e4acb2c34737d54def64bf0fc9483689e570118a92a4c8e8dcdb`  
		Last Modified: Tue, 14 Nov 2023 02:56:03 GMT  
		Size: 8.0 KB (7983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d5a662bad6f856ef312d0020468797abb4291aea00c8dd1494390c9e51c6eb5`  
		Last Modified: Tue, 14 Nov 2023 02:56:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:777a56017227fc7efabb2e2173ab65c9b46ffa9c082ec537da06cbb7f1fd2431`  
		Last Modified: Tue, 14 Nov 2023 02:56:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:546af9961cd67953034166fa49286640b50a816d447d87e365edf007e961c116`  
		Last Modified: Tue, 14 Nov 2023 02:56:04 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:df9fd179e22053e6074ffa01cdc47658fcfdad5361fb6a05158982e30dd00334
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.7 KB (838722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4122961e03bf2ced4660f3dad213dd5bb564cfddf99462f4903b1d17eb60406`

```dockerfile
```

-	Layers:
	-	`sha256:c4a449dbfdbf207f0cdc9127d3e5af7172276cf2cfd8f8f9ec1b7ea94f6cc6d4`  
		Last Modified: Tue, 14 Nov 2023 02:56:03 GMT  
		Size: 803.1 KB (803123 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d409b15344a202d9f79479b0b4921c7949f42e440dd6b70decc983dd4fb7af0b`  
		Last Modified: Tue, 14 Nov 2023 02:56:03 GMT  
		Size: 35.6 KB (35599 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:ccd564f15deefbb70a640c365613bf0da04b764fb7788b8591b146fd1fec27ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93161955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f2e0d1cdb1124923d0c1d377ff540f3d6c3c3967c0792aff805141a79f65b4d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_MAJOR=11
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_VERSION=11.22
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PG_SHA256=2cb7c97d7a0d7278851bbc9c61f467b69c094c72b81740b751108e7892ebe1f0
# Thu, 09 Nov 2023 19:02:26 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"11.22","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@11.22?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:02:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:02:26 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:02:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:02:26 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:02:26 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:02:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7ae232bced3defb4eae7f5affb566ea50f50655d575488965e418a8da86b3ed`  
		Last Modified: Fri, 29 Sep 2023 18:03:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68a6f64e487e2750fccb626c86600fd10e0346eabb9bdb31da4b7824cac4a0b`  
		Last Modified: Fri, 29 Sep 2023 18:03:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e99d487cac0a45397748be7d4b4fec8daddd586ac8631948a5c939802dfb2d3b`  
		Last Modified: Tue, 14 Nov 2023 02:21:50 GMT  
		Size: 89.9 MB (89932397 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b19b052d7aaac7c4409ab8218d817af4367933d6d58325e9ee344f28fc48dfa`  
		Last Modified: Tue, 14 Nov 2023 02:21:48 GMT  
		Size: 8.0 KB (7988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b0f9c0c7f7715cab38e12d5854c86ef69dcc184918420ac0c7e46e89481b072`  
		Last Modified: Tue, 14 Nov 2023 02:21:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb16f2ebb73552724df099793acb5ae279a5b1b9df44f0c9994e1ae178f356a1`  
		Last Modified: Tue, 14 Nov 2023 02:21:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f49242927c2845252eda66ec97b9f09a416a5032bb89a70b7e0855839b9d18`  
		Last Modified: Tue, 14 Nov 2023 02:21:49 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:5b082c6f79aa68e7a106d2b8bb2fd804f44b29562a37b9d8754d1678c489c744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.1 KB (840055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a08edc072bc9de55a5724366e89e7d01025a3855ce2cc67defeaf7dd3ce87b4e`

```dockerfile
```

-	Layers:
	-	`sha256:d17e700ec6df96dafb31c326292f90756b418019205c5ca92ce82183c727f142`  
		Last Modified: Tue, 14 Nov 2023 02:21:48 GMT  
		Size: 804.5 KB (804504 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2f1f543a52539f0e92692fa62bb798db3e43c3406b647c3d71b8ecd4196a3a11`  
		Last Modified: Tue, 14 Nov 2023 02:21:48 GMT  
		Size: 35.6 KB (35551 bytes)  
		MIME: application/vnd.in-toto+json
