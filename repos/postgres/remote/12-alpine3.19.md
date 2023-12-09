## `postgres:12-alpine3.19`

```console
$ docker pull postgres@sha256:9b962f3baa54abcfc4c6c13ae24dd758fc5dc706c3a488ff8a1286f8a529e65d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 9
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `postgres:12-alpine3.19` - linux; amd64

```console
$ docker pull postgres@sha256:5fd78fb10ffcb7323db1950bad3d166b64555659c38d424cdd3efe0c1091d70e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (91958878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6ed760edc243194c1fb658902d16628a81191013c45b11c424cf9abc877d2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV LANG=en_US.utf8
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_VERSION=12.17
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Fri, 08 Dec 2023 11:47:00 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.17","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.17?os_name=alpine&os_version=3.19"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 08 Dec 2023 11:47:00 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
STOPSIGNAL SIGINT
# Fri, 08 Dec 2023 11:47:00 GMT
EXPOSE map[5432/tcp:{}]
# Fri, 08 Dec 2023 11:47:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18c428da476adf71f2197b6888cefb8fc1cfeca5acf1abdf9e2af8ea9f3fd311`  
		Last Modified: Fri, 08 Dec 2023 22:16:14 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5103370bedcdfece72aa566d957e6ba21f178f681ae319e3a7a71f41f79e5cd0`  
		Last Modified: Fri, 08 Dec 2023 22:16:14 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5adf99d247f83b7681045116ca5dbef5fefc3f4e392ec48663d9166067e9782f`  
		Last Modified: Fri, 08 Dec 2023 22:16:18 GMT  
		Size: 88.5 MB (88535258 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed41abc0acae0b241f559c0369efb884ba12b4b9605f5959e24e9734427f0a29`  
		Last Modified: Fri, 08 Dec 2023 22:16:14 GMT  
		Size: 8.7 KB (8686 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45106b3e43da11ef5c1c57f36cca492cc35c15f81abe4db5107aaeb5a379219d`  
		Last Modified: Fri, 08 Dec 2023 22:16:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f877520037697ebe9adaa3e0e67c67bb48e246d58b1d188ac10f49ffd982402`  
		Last Modified: Fri, 08 Dec 2023 22:16:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d2b9e3dd93bbdd3e0d378a809bbd1c3b01102daf19f6b8d45c006c92692dc2a`  
		Last Modified: Fri, 08 Dec 2023 22:16:15 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:c79f69fb1c10683e360741925c6c9797564b3c94947848b68cc980299bd8454a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.5 KB (841500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7880fd17c9d25e0a1f30c841ec727f266922deb009857790836d6832e4071b18`

```dockerfile
```

-	Layers:
	-	`sha256:ca2884feae668fcef925313abb2f495d1db40d83081b65cace9cd4850ece90cc`  
		Last Modified: Fri, 08 Dec 2023 22:16:14 GMT  
		Size: 805.8 KB (805780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:de50d383bfe7ce02a4f0848222bbc10970910a44baa0b83bfa0d91bcfe93608e`  
		Last Modified: Fri, 08 Dec 2023 22:16:14 GMT  
		Size: 35.7 KB (35720 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; arm variant v6

```console
$ docker pull postgres@sha256:1ffb380ba0e01ffc3a0f3ed0b448f2c2b2a6e3ce8ed138538b997a122c9b2607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90860089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbd08d5c12ad9ee4f603089b421908393fb84a43c9df1dec58d02b121a15499f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV LANG=en_US.utf8
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_VERSION=12.17
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Fri, 08 Dec 2023 11:47:00 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.17","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.17?os_name=alpine&os_version=3.19"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 08 Dec 2023 11:47:00 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
STOPSIGNAL SIGINT
# Fri, 08 Dec 2023 11:47:00 GMT
EXPOSE map[5432/tcp:{}]
# Fri, 08 Dec 2023 11:47:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fe015dc9b3d1803ee85ee6a801a8a7e2d6311686b2f37622ccbe41860d2ed3`  
		Last Modified: Fri, 08 Dec 2023 23:56:18 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a72ec48bcaaa26d249e92564caffd5723eebb17b13de29d037b52a50729964c`  
		Last Modified: Fri, 08 Dec 2023 23:56:18 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79dc5587ee63a916220998aa5394bb89c8bebf1f707961b6c92459caeadd523c`  
		Last Modified: Sat, 09 Dec 2023 00:22:52 GMT  
		Size: 87.7 MB (87679800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b773a44c7932ef2a9fc5c45581d6b229ddfdff62cbb288bd0c4cea60c9875ec4`  
		Last Modified: Sat, 09 Dec 2023 00:22:40 GMT  
		Size: 8.7 KB (8686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631a4a49648eebcc75451c286f8c037ae52a6ca3f91a3c1dac8103749c9dd4c9`  
		Last Modified: Sat, 09 Dec 2023 00:22:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa79efb398f86580882cdef7396c69420dea340f0e8f4163c4b39713d787308f`  
		Last Modified: Sat, 09 Dec 2023 00:22:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50394c3c3618a269dff83db46924b433280840306a114f0d1f903d44c68ddf`  
		Last Modified: Sat, 09 Dec 2023 00:22:40 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:576a0b8792c72bad1620892057aff8392286cbb62cfaf2490eaac025e157f336
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90799100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccaa04f2c5dc7fe7eb36f8094021221163dd5c95719f1f0652e155a981d09f38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV LANG=en_US.utf8
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_VERSION=12.17
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Fri, 08 Dec 2023 11:47:00 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.17","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.17?os_name=alpine&os_version=3.19"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 08 Dec 2023 11:47:00 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
STOPSIGNAL SIGINT
# Fri, 08 Dec 2023 11:47:00 GMT
EXPOSE map[5432/tcp:{}]
# Fri, 08 Dec 2023 11:47:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95b04ba977a6ee37b8b3c87adac565605b88cfec398fd4daf97fa685414e2ef8`  
		Last Modified: Sat, 09 Dec 2023 06:37:26 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1e0d29db9882cf21901e330bd0ffb89af524dd251a76d114937364110879528`  
		Last Modified: Sat, 09 Dec 2023 06:37:26 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc8f8851f0f5bf65546117b4e846597d8365524c036cc101974dd6ef87f8ca21`  
		Last Modified: Sat, 09 Dec 2023 07:05:05 GMT  
		Size: 87.4 MB (87436160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5898fdc09064c94a7c41c5d6e44baba3cf86e35d1c98d94f71339082c6aa298f`  
		Last Modified: Sat, 09 Dec 2023 07:05:01 GMT  
		Size: 8.7 KB (8687 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f23ebfd5ed7cb57b7bcb68e7aea6f6f80906ca719d100616593b2acfdd1cc21`  
		Last Modified: Sat, 09 Dec 2023 07:05:01 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4bd692293ddad9e14a77b44213d2495171d0f47cc209f4f1594d9e5d46dda59`  
		Last Modified: Sat, 09 Dec 2023 07:05:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15b3b372d952365d4962f0315c7cf500d229428c705d86470b9ba7e46a78beab`  
		Last Modified: Sat, 09 Dec 2023 07:05:02 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:0fb3fa9b8550d649f0585341e18f1f7f5e9ee07469cb85a4bfebc40d44fdffa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **841.4 KB (841356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:817278113d981c641d9e20b2c4393dde41d077da39f28cb353930c7400da47a3`

```dockerfile
```

-	Layers:
	-	`sha256:d824604f0f3a0f2a2cec79ea823200df5e71b84958e4745a11065c1f8c87afbe`  
		Last Modified: Sat, 09 Dec 2023 07:05:01 GMT  
		Size: 805.8 KB (805791 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b7e19f502fd2c1824a308cc4e1b09457cdbf3d6a49db34bfa0134318989419c8`  
		Last Modified: Sat, 09 Dec 2023 07:05:01 GMT  
		Size: 35.6 KB (35565 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; ppc64le

```console
$ docker pull postgres@sha256:93bf31d3760122f342df5f65b75e56fe21709520b76a978742fd67e2de13ad71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96421480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:244cea983e2e0435dad624859128a3467facc663e4e4d1c59d4497161208ed38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV LANG=en_US.utf8
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_VERSION=12.17
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Fri, 08 Dec 2023 11:47:00 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.17","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.17?os_name=alpine&os_version=3.19"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 08 Dec 2023 11:47:00 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
STOPSIGNAL SIGINT
# Fri, 08 Dec 2023 11:47:00 GMT
EXPOSE map[5432/tcp:{}]
# Fri, 08 Dec 2023 11:47:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f51ffbccda0d404d0ffeda33fa1a948c925d8f36f5899665a15528b160466a7`  
		Last Modified: Sat, 09 Dec 2023 04:46:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4c6b15c27b5856f2fea6198b0dfc83bfee906d7b94102503c986f1e789b8dd3`  
		Last Modified: Sat, 09 Dec 2023 04:46:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e660400f09ea88122d30e4d3b3d8cf4fcbc81cb52554c4aa3dd080ee7eda3597`  
		Last Modified: Sat, 09 Dec 2023 05:32:44 GMT  
		Size: 93.0 MB (93048096 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91a5fd56c4c63d0111212df6edad46daa6b42401ef09f02de1b923b151266707`  
		Last Modified: Sat, 09 Dec 2023 05:32:42 GMT  
		Size: 8.7 KB (8691 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5303c6c19c53bfcc289cecb875b9af9b0949ae8ba4034e835271630a818d3823`  
		Last Modified: Sat, 09 Dec 2023 05:32:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f116d1eebf969a89acb1bdd2ae81bce29082f8d572901ed7468ea3bad19023c2`  
		Last Modified: Sat, 09 Dec 2023 05:32:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7adf6bb79fac768f669cbcc785ec178d80c7958ec44361506a6f97bfee8ded38`  
		Last Modified: Sat, 09 Dec 2023 05:32:42 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:e40070cc43200e3f52a70257db8558aabb96a3247b25679655a12040ae571505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.4 KB (838366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7915fef2d8409b2261d8d083810a7d827b2ed547fb7f92cc008192141bb96a3e`

```dockerfile
```

-	Layers:
	-	`sha256:a608ab46e53ec0a6185abadf63e4c91f87e645ddd9376cb1a6ff481811260df6`  
		Last Modified: Sat, 09 Dec 2023 05:32:41 GMT  
		Size: 802.8 KB (802763 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9782c7c707b95b48c7699d3761ab366cd7fe856d7a3601403fd112c5e68a5fcd`  
		Last Modified: Sat, 09 Dec 2023 05:32:41 GMT  
		Size: 35.6 KB (35603 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-alpine3.19` - linux; s390x

```console
$ docker pull postgres@sha256:262dec17dd153d7af414f5a297c2f5e3abad2678b299c5e836b02c44424a613e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100692713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:567916f30b131b09da283be2e183a552ae2f674af5187ead50838922c6cf2d04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV LANG=en_US.utf8
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_VERSION=12.17
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PG_SHA256=93e8e1b23981d5f03c6c5763f77b28184c1ce4db7194fa466e2edb65d9c1c5f6
# Fri, 08 Dec 2023 11:47:00 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"12.17","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@12.17?os_name=alpine&os_version=3.19"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 08 Dec 2023 11:47:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 08 Dec 2023 11:47:00 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 08 Dec 2023 11:47:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Dec 2023 11:47:00 GMT
STOPSIGNAL SIGINT
# Fri, 08 Dec 2023 11:47:00 GMT
EXPOSE map[5432/tcp:{}]
# Fri, 08 Dec 2023 11:47:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98867b7d9ef52d8ea690ad6ab7a1162c3ffb223f498cfe46c5a0c19b26b5df4a`  
		Last Modified: Sat, 09 Dec 2023 02:05:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eca1d0e320956171da67959a489db8954c94e3093132a48ee544fcaf765d7784`  
		Last Modified: Sat, 09 Dec 2023 02:05:53 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5686976ae6d89ff0193dbc4cec02015507da08006515cfe2192202a4e2441e4d`  
		Last Modified: Sat, 09 Dec 2023 02:36:28 GMT  
		Size: 97.4 MB (97435235 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0dbe4e0e5c55c0618d4a3c67fb04b8ed773ae503896035629c7e9e32fde1297`  
		Last Modified: Sat, 09 Dec 2023 02:36:26 GMT  
		Size: 8.7 KB (8687 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b584c745a106e397b167f1ea5ca968f80dfb1aa0aff76f3fad9caef45b75ef7`  
		Last Modified: Sat, 09 Dec 2023 02:36:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09c3e5ab3ca1f5eedaa09097737f494dd0eed085fb55e0ebb4b4adba6c0681a5`  
		Last Modified: Sat, 09 Dec 2023 02:36:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09da6a898e3c5d4980d46512fc397c9b0084c4423d36561c26eccbe649bd3b13`  
		Last Modified: Sat, 09 Dec 2023 02:36:27 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:be58a36dbcce0f82fff26d011a383aeb6f9bcda0bbfe96b23e27b682029d36aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **839.7 KB (839698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df964d16452c61cb8fbb65abab7f1fd71807e9326e6e981932de5485c50dd48`

```dockerfile
```

-	Layers:
	-	`sha256:2ee7449017740fd75ea83d90a2ca782da501ec3104fa745a3f84f183f6f9c02c`  
		Last Modified: Sat, 09 Dec 2023 02:36:26 GMT  
		Size: 804.1 KB (804144 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e5f4467acb48b0351eb5ea1bb682cff909ee657ee7957dc678180d9829c08538`  
		Last Modified: Sat, 09 Dec 2023 02:36:26 GMT  
		Size: 35.6 KB (35554 bytes)  
		MIME: application/vnd.in-toto+json
