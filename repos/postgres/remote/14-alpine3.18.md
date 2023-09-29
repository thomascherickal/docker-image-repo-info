## `postgres:14-alpine3.18`

```console
$ docker pull postgres@sha256:78f88886f81ba4c813f1f98553a742c063348c6622416dfb5190139a80b71591
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

### `postgres:14-alpine3.18` - linux; amd64

```console
$ docker pull postgres@sha256:9d0c2cbdf10088d633876f01750d077b501bf258517ad04e486ddb2f4206486f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92725630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf1eee232f3319381cc820134beadbc0b2c5a09060829c5f80863a24c0f4324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4e10cffecccf55184eaacdae8d9fd0b7639ddb3864b4b8d19d2111b33daf1310`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbd7fcd11034c95a6a2a35673030f66b23620d50b5389c1e70a89fcad1593ad2`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcd80084e9e579b0c34fea711c0a449acacce93cb75171d0f0e61d054c4a4140`  
		Last Modified: Fri, 29 Sep 2023 17:14:52 GMT  
		Size: 89.3 MB (89308002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ce5f36afa1c4a30ae7be2b2c525115ac244e6b5f8223455b7fba70f97cb7795`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 9.2 KB (9199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e9f23f76af6246fb8d612378d00bc1897f9f7c9b64905b21005e99803c74428`  
		Last Modified: Fri, 29 Sep 2023 17:14:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a527d48a0f567ffc0bed8625d83265815c301620fd44a7229c169af69ccb6dd`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9720076694ec4a64e4af1d10933b3339fe0b2b54c7a6a82e4ae38083a42370c`  
		Last Modified: Fri, 29 Sep 2023 17:14:47 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:9732d7dce94a63d901cc8e9941d3e5ce74716db5a98d2fe79e3c085ce3dabd4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **869.8 KB (869829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52f3c4595c3d678f6d5f1f5759ec7ee73158452d633c8b4c3b6d5924b4d3d813`

```dockerfile
```

-	Layers:
	-	`sha256:a53ba0c724352bf822cf8f990d936bff0c6562648df9cf0420978ea261faf674`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 834.9 KB (834880 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6f874b11295633ebeaff5094412e49dcbdc1fb9f7a10003d1a1eab680b395898`  
		Last Modified: Fri, 29 Sep 2023 17:14:46 GMT  
		Size: 34.9 KB (34949 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:b6ce5cd96255426357af0e4b7e8a9f0883ebf4220e26ccecab3fe556184cbb8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.4 MB (91427129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a8dbace21dfe76523505a281fa2151828ad136ddb212edc175a8f17e352bad9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f9677461cc1446c142c4f11c5e5ba7ae5eb0160b5884c6c4703d8bbc271706`  
		Last Modified: Fri, 29 Sep 2023 17:11:50 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da301824fff35c4518ffe54b8851eeba7f52fe7519c55c3daee52a26301b52c`  
		Last Modified: Fri, 29 Sep 2023 17:11:50 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edab2e85eae36ee874d1d9311bd993ba98f018efa642e41b2605442c451ba8c`  
		Last Modified: Fri, 29 Sep 2023 17:27:05 GMT  
		Size: 88.3 MB (88266178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c8652210562fb91216670e153b344fa2676385bed6f6c10c6f3554d7f715a6`  
		Last Modified: Fri, 29 Sep 2023 17:26:53 GMT  
		Size: 9.2 KB (9201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2114ac9d9d67bafe2f1f4a408679a93ef33b058c51d55a9bb522ca7f45f8a961`  
		Last Modified: Fri, 29 Sep 2023 17:26:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc21dfb63da8e7569f2b5f010298ff5de91c710e21e79554b00f9c95a5bd3079`  
		Last Modified: Fri, 29 Sep 2023 17:26:53 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45522c8aabe96879bb365f36fc7bd6f14607130d9c60545dd6ddbb10f95fb4f`  
		Last Modified: Fri, 29 Sep 2023 17:26:53 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:7739fda9a8442486c99d4fb466335c23053e55a8b09ea5e259964b9575b8e180
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86102664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d12aeb86552ccd3d1b26e12ccf1cfbc096dd5c0b823c1cca08ad5c1d057e2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
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
	-	`sha256:dc26c5829aebb87ad99b88fa12121fe9af5fadc9a1cf3284276d5dda9d83cbbe`  
		Last Modified: Fri, 29 Sep 2023 21:20:19 GMT  
		Size: 83.2 MB (83187103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae5a948caf420b53171f81451ea1d307cd22cbf0b5d24be45a678b68c13f32ca`  
		Last Modified: Fri, 29 Sep 2023 21:20:14 GMT  
		Size: 9.2 KB (9200 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2c3faf77976623f031e1a932d43324eab12af9a4faddb4eee297aeedc325930`  
		Last Modified: Fri, 29 Sep 2023 21:20:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad6d4f91cf06031111ae29c321b2501461b03d50b83157cc18968a2a7ef2c14f`  
		Last Modified: Fri, 29 Sep 2023 21:20:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:173030590586295533de11f9a715f795da19455409d2055dc70dcfd476f0e0b6`  
		Last Modified: Fri, 29 Sep 2023 21:20:15 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:4a996c7c6d0d235ada93dad9914fc14bd06db9f23817f00ed8bdb93414da8cfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **869.8 KB (869831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0761bc89f4d7ddbb82739f8b0c7acc27e8574b563f6724cf87ca73b2ed434ac5`

```dockerfile
```

-	Layers:
	-	`sha256:aadc5a9964bc7c5997448c322f998a8c879dc5f1fd87a58c6d0b5765354b2074`  
		Last Modified: Fri, 29 Sep 2023 21:20:14 GMT  
		Size: 834.9 KB (834914 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c3844596c45a742d540ad27e719e118c9bdcaa9dce6563e810eb73eba6ddda1a`  
		Last Modified: Fri, 29 Sep 2023 21:20:13 GMT  
		Size: 34.9 KB (34917 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:8e6faa7eefd498ddc94f67ac2f8fd170d7049d8499010498ecf5d691a0f2a1c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91687199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dc66e6ce82907258e62dcd9798ac96237509d423df1f80e2a69a05b3f0179d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
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
	-	`sha256:fc0ad1f441661d059b5ec3ed0aa5355689ec8963c141f08bfa735eed166ea009`  
		Last Modified: Fri, 29 Sep 2023 17:28:36 GMT  
		Size: 88.3 MB (88339711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ac7aaebb3c918b8ae07fb594b02713b42825a2e82261bcd03e5c0dd78e61b4`  
		Last Modified: Fri, 29 Sep 2023 17:28:31 GMT  
		Size: 9.2 KB (9199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6482e4241bf802fbe629cd944f6d565db72d34fe01914bd097a4ea31465d5cf`  
		Last Modified: Fri, 29 Sep 2023 17:28:31 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40abf5cf6bac45254eaa06bfe1598793b144b1f9f5c11051d9d093523638688b`  
		Last Modified: Fri, 29 Sep 2023 17:28:31 GMT  
		Size: 167.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37a6c32bf1be2576828197ede75b66f1b463491b1149edc5e732d4536bdc5e09`  
		Last Modified: Fri, 29 Sep 2023 17:28:32 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:9e6427696ead02b63096f836336243d6173a37be79c6603777df6982da9cb6ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **869.7 KB (869686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63701632f0cdc8ad89a010667988e55258cc86c8f09bfd22dc21e8d5381d9100`

```dockerfile
```

-	Layers:
	-	`sha256:85ed5aa74e4bb712b6f20be02abef8dbd6de911f0123f9b4c88ebc1d5778f6a0`  
		Last Modified: Fri, 29 Sep 2023 17:28:31 GMT  
		Size: 834.9 KB (834893 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:25ceefefb7ed09eb31794bc012fbd96a368339e83faac59e75bf095e9eaeeab6`  
		Last Modified: Fri, 29 Sep 2023 17:28:31 GMT  
		Size: 34.8 KB (34793 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-alpine3.18` - linux; 386

```console
$ docker pull postgres@sha256:e21b99249100b67e948899a172af1e95e02917ced2b3dcab44ffc8b49d22c49d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97708357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:035e67419baf7df64ced27984969ffafa25cafe4f07abd4bcca804838612d747`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9dbb33f95544ccf2ffc9ef0012eabe4215ea5965ff84a47e71ad41c39a36191a`  
		Last Modified: Fri, 29 Sep 2023 17:15:23 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96c52c00abf0b5c55587a4a241386e89ddfcf0cc11cba54dce2c0b21eee91592`  
		Last Modified: Fri, 29 Sep 2023 17:15:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea931c90eec9f14658c1a9b04d356d5fbd301cf1e92f9255480a46cb677f49d6`  
		Last Modified: Fri, 29 Sep 2023 17:15:29 GMT  
		Size: 94.5 MB (94456938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70812d2d529016743982dce14aab120380fb6c9466d559109b44cf29e4a887e4`  
		Last Modified: Fri, 29 Sep 2023 17:15:24 GMT  
		Size: 9.2 KB (9200 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4fa1afe740ff4d57527d971e9c6ec967f2cbeea7842233ed5a21d7339f605a9e`  
		Last Modified: Fri, 29 Sep 2023 17:15:25 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a1aaa0998c3d178f0b0586b6b8e212372465cbd80f17263d0cdb378c4d047a4`  
		Last Modified: Fri, 29 Sep 2023 17:15:25 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8065a2d584f5264ff8729cc835dd259faadc48b3ad4a4377dd4e7808b7ce6e3f`  
		Last Modified: Fri, 29 Sep 2023 17:15:24 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:0dd79c41a1da3e7ea5266546db457574cf5ff1757229bbb8f073818c82103cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 KB (34694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23d0700b41e7e4d7be03fc6937ded6fea1645b53979e159c889f6ce8fcaab62`

```dockerfile
```

-	Layers:
	-	`sha256:92028c9bb783fd76c49ad4c4c8571ae7ce6d9c0e001308957dfd6e2317501611`  
		Last Modified: Fri, 29 Sep 2023 17:15:23 GMT  
		Size: 34.7 KB (34694 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-alpine3.18` - linux; ppc64le

```console
$ docker pull postgres@sha256:04e4eb44b8f081c77ee9b8486449d97af6c53a637ce1032451aef77d1bbc5870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.4 MB (98360616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3367253eac7f84aabb8ef14cd43ea01dbf03a8224fecc3df31f41b0cec8d8055`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
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
	-	`sha256:352def4a387f04d106c07801562ed9f0ac58ffc94e549652f52d1555908a460c`  
		Last Modified: Fri, 29 Sep 2023 17:47:00 GMT  
		Size: 95.0 MB (94998436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a213cc0aa8efcb9d3a2a59e73b481eb36032a3c81403465c394aa75bafa418b0`  
		Last Modified: Fri, 29 Sep 2023 17:46:57 GMT  
		Size: 9.2 KB (9209 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2f4ab2f6c9b47b18421e31dd53fbdf2bf4c1ecb49502af202cc85de01bdc6e7`  
		Last Modified: Fri, 29 Sep 2023 17:46:57 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e8a0dfc14f271ec20ae86c2a83c64b318afa550d443bf597c024fcb353e7334`  
		Last Modified: Fri, 29 Sep 2023 17:46:57 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f21389f4636d6da7442cefa5d97840c735d91fab1a14b7697ffd8e25499b82af`  
		Last Modified: Fri, 29 Sep 2023 17:46:58 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:1f5d61f60108a6b72956d1d04d72c9c1b1849b1fbb6ac84e6023ea36d5f25098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **866.3 KB (866316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d66a1f07aca7d61bd5f4c218c3e2a41f27457e2a7a3268fa672742c7af811dd`

```dockerfile
```

-	Layers:
	-	`sha256:ad7f1656034dcd576f1e815047909ec0f1bc51bca2fe882f241f5322cd87da60`  
		Last Modified: Fri, 29 Sep 2023 17:46:57 GMT  
		Size: 831.5 KB (831485 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d16682f6f5e8026ce11d5bb7ff3d70180a3c597afdc9703823c8c609af6202e5`  
		Last Modified: Fri, 29 Sep 2023 17:46:57 GMT  
		Size: 34.8 KB (34831 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:98c32a56dd838c1917a46ef22fc71fa338bf643eef53ced40a40a1c1a3580369
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.4 MB (94368072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574eb7cf3daa331c03185eae2d8c3b3d2b062eae07bf24b0991d2a03075c2994`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["/bin/sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_SHA256=b1fe3ba9b1a7f3a9637dd1656dfdad2889016073fd4d35f13b50143cbbb6a8ef
# Thu, 10 Aug 2023 18:35:14 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
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
	-	`sha256:93eb02d90a124a96bc6a3892a861adfbc8cea1cf2d07237f816b03287ed6eb45`  
		Last Modified: Fri, 29 Sep 2023 18:24:56 GMT  
		Size: 91.1 MB (91137304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:568554aef43d42926f55918dfa20227125cf99f5b44bd70f5b38212651affca5`  
		Last Modified: Fri, 29 Sep 2023 18:24:52 GMT  
		Size: 9.2 KB (9203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26cad06215e1b96b3565182c1f347f90b3403813584bfe0e44d0f3e0a4ee06f0`  
		Last Modified: Fri, 29 Sep 2023 18:24:52 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96cd9f751254d55a650e507e7957cf3cd161e4f798fd3039b04a43ee65097b1a`  
		Last Modified: Fri, 29 Sep 2023 18:24:52 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5eb296c5847a87060632d12f2d7f11061609f6ff7da3d01442e5b29713051b7`  
		Last Modified: Fri, 29 Sep 2023 18:24:53 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:c64daadcc9a5146d6aa1e5f4b0d29fd0ce65daf7cbac96ff1d1e60c3d75cd679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.7 KB (867731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1a319debfe93bcb73182035c23d4d5836900c220729bf1f7c8714d0df9c289`

```dockerfile
```

-	Layers:
	-	`sha256:19ed4a287216c9a46222b5866a10b3be0ce9f386918fab8cad90735fe2358943`  
		Last Modified: Fri, 29 Sep 2023 18:24:52 GMT  
		Size: 832.9 KB (832948 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bea07bae13eddd489856a1bdd3b161edba1ae0fbc0bb7d3055b2dc6109e8f338`  
		Last Modified: Fri, 29 Sep 2023 18:24:52 GMT  
		Size: 34.8 KB (34783 bytes)  
		MIME: application/vnd.in-toto+json
