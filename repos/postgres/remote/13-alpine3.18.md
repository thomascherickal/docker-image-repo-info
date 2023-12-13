## `postgres:13-alpine3.18`

```console
$ docker pull postgres@sha256:9b08b85599e35706b0097b30513a62d9ad0119f54d46eb966a904409eee91275
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
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

### `postgres:13-alpine3.18` - linux; amd64

```console
$ docker pull postgres@sha256:d0accbb1525e057230cb9b1a78e80e196d0ae55977ac8e0bf381832e7d1119da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91244660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4bd206a126da7c1de2bb69c8b9ada533631f51af34653a8f8d5342fdafebe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1f17320fb30a4211071d2daa990d26b3e855b9bf95f6ca9a33bd979e9ecf8e8`  
		Last Modified: Tue, 12 Dec 2023 20:53:44 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10c5456245df1b56a725471c50402ca9bc3ef5f97c3ddcc9f272a54966d02704`  
		Last Modified: Tue, 12 Dec 2023 20:53:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:689c115ee6a47a5067d774449425f95907a0957ac997c6b0618dc6edc973abe7`  
		Last Modified: Tue, 12 Dec 2023 20:53:46 GMT  
		Size: 87.8 MB (87826754 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a8838aefeae4e7c882206a3f2a0ccbe434bc5f240c0b3e61eadfb1c05c3d11d`  
		Last Modified: Tue, 12 Dec 2023 20:53:44 GMT  
		Size: 9.0 KB (9020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f8b9ca4cfd6f1e67be2392fcba5581e44f39b53206a9ee05c09cb5413b61d8a`  
		Last Modified: Tue, 12 Dec 2023 20:53:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8a1f421efa739dbadc943d37147d34f8c2d9a3b84ed6640f1ef27268eb872f6`  
		Last Modified: Tue, 12 Dec 2023 20:53:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d57142e86a1b194dc094cad88eaa746fd7deaf412182845520b3e0146a6c5a09`  
		Last Modified: Tue, 12 Dec 2023 20:53:45 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:912fe3a7e0335301f8e7f449a927bada59037ef6fc2a219ad59f55d5b3672fff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.7 KB (837690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cda1533c00eda982ca33daed0da1eeb56f80dea2054784fcb84c7e455cd78e07`

```dockerfile
```

-	Layers:
	-	`sha256:fa52eb9a6dfb2c3cfa00491e088d24078cd4273946f82b315553debefb180062`  
		Last Modified: Tue, 12 Dec 2023 20:53:44 GMT  
		Size: 803.6 KB (803632 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1733496936d7ac1d93562f76b44a862f1dbcb3b419c4dee8d3c97d7736ceb1aa`  
		Last Modified: Tue, 12 Dec 2023 20:53:44 GMT  
		Size: 34.1 KB (34058 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:aed711d519e48e3fc00b682d45d29b1240a6016c431a25e414fb7a46ef13c7cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (89967283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7fb7331c476ab01babc1fe33cc9a8a56583d60e4846bbae26e928e256c7d63`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99733932520adb79e9efc69d2e2eb3fdcf866ff3f27e44c498d477613b8f1009`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8563d30a0024e9dd3241d3e57d864c72dde0de3fd4903d603de211fd26738a22`  
		Last Modified: Tue, 12 Dec 2023 22:40:38 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da1a5c0a65b0369dd8abe78c72a4d589f437be8a4cefd675f38573354d3fe3d5`  
		Last Modified: Tue, 12 Dec 2023 23:57:31 GMT  
		Size: 86.8 MB (86804937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d2e004fe7593acfe74ba1bcc486fe44222b0e18079eab2ee10c4e93a92c7de83`  
		Last Modified: Tue, 12 Dec 2023 23:57:28 GMT  
		Size: 9.0 KB (9020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77be8bafd6aa8637e31e25cce45d72c7f03a47e736b605de30c7840c7e2df55a`  
		Last Modified: Tue, 12 Dec 2023 23:57:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bf74140f23b84a39a2a0dc0b65257b9ab7f987bbc6db91aea6003beb81302b5`  
		Last Modified: Tue, 12 Dec 2023 23:57:29 GMT  
		Size: 167.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a6d3b84c0612228cb5aac8e79191a36ed6715d7a572b0ad9e880a0388dd5084`  
		Last Modified: Tue, 12 Dec 2023 23:57:29 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:d152108d5bd6d9daf280422dfb4b071bcf46e47b8f4926385ad997f1e5ca37ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 KB (33796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b24df1e92c398f654c93e10d5ca9ae9990e00ff6c1018ef8db002a2b47aab51`

```dockerfile
```

-	Layers:
	-	`sha256:7a9c2c317acf5923d947cc72f6bfde3c657697f4c3b64b0b0522b612b604dc87`  
		Last Modified: Tue, 12 Dec 2023 23:57:28 GMT  
		Size: 33.8 KB (33796 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:fc5d08e3618204bb1b6e622ef8a6af03f81188cd7f8baeeec1b7897b183c21a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84671538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f47e8d9f5d7c134b98d6980b8faba8c603abefdbaee7121d38f9638d19abb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c815d47e00d2d70d22df505cd75fee458db7a056e91cea2be9e903be7b3cf887`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cc211333283e058626a589bb51c6eea6895cc4988e59b83890811a76d7be3a1`  
		Last Modified: Wed, 13 Dec 2023 01:53:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38f65f0fb341283f0b2735ef5b74da322353e0d8e78ee4f163fc0d2bcb1be964`  
		Last Modified: Wed, 13 Dec 2023 02:14:11 GMT  
		Size: 81.8 MB (81755050 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b67f68d97247ca33363808a68149a45961c807c7b458868601ef89dbf55fa65d`  
		Last Modified: Wed, 13 Dec 2023 02:14:08 GMT  
		Size: 9.0 KB (9020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba27079cac4d3ff067e5d48f53e53c73b1d06ea803bc4bd04fceca18e6ced541`  
		Last Modified: Wed, 13 Dec 2023 02:14:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:877a1b1659250dce72bf04ed7fef9c043ec09eb9fcae4f5ed9380f21a4aa0b03`  
		Last Modified: Wed, 13 Dec 2023 02:14:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:911cb007d467b3efd67732a352b5760c81d589fbc2f04b0078ddc9e87582590c`  
		Last Modified: Wed, 13 Dec 2023 02:14:10 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:82586497d334aaf289e807e2963eb7c2fc2c5297270ab064a30192113380e293
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.7 KB (837663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8485a0d0bad40ab80c346337a55b63e1ffd75f4d68ce2b8bf113f40a248b19e1`

```dockerfile
```

-	Layers:
	-	`sha256:b93c7f6071e69e043df87b1d8a53d8983ba752f9b7ed7bcd362676572e95f674`  
		Last Modified: Wed, 13 Dec 2023 02:14:08 GMT  
		Size: 803.7 KB (803652 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ae89c7c0d8247cb17baa8241fd8a87f735e7c4c0770c798a99464ba8bb66b012`  
		Last Modified: Wed, 13 Dec 2023 02:14:08 GMT  
		Size: 34.0 KB (34011 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:cc0e7bc05622eed3068cfa7f73fc87616729564817c0be1783022230f3f2c533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb68b85b3d161183760f3f5d8989fd09d9d6069b580de75650f38ddba089a752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f976195ad28258b2cce8a3feff1817f99cc57aaba200954d184c38814d91795`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03936fc3c66b1d124f91e7128a308d9c4de24f1374198667f3b5dcf9c8a0c88c`  
		Last Modified: Wed, 13 Dec 2023 03:03:02 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f82db9dbf7d888ac095f833861dc7f0d6ab2ae8c489a5346fe19ca0049ae0374`  
		Last Modified: Wed, 13 Dec 2023 04:20:07 GMT  
		Size: 86.9 MB (86873655 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73491a8ed6f25963123f8400afa0a298c7cb6d1dbb53763f94368c64dafc7c5c`  
		Last Modified: Wed, 13 Dec 2023 04:20:03 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b8914db02727251e8b7fd348aadce64f88f2ba9bd81436016a3f5dd0cc38618`  
		Last Modified: Wed, 13 Dec 2023 04:20:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74d27bd620ff27daddedbad8a85ed80dbb73f6c33816b4a98c5cb9eee830274b`  
		Last Modified: Wed, 13 Dec 2023 04:20:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e44e946054b92f0cd6296f03d220d58b1cc4a276f590ec568ff2c14f61f9a9e6`  
		Last Modified: Wed, 13 Dec 2023 04:20:06 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:160f47116d702b444fd7abd96f94ecbebdbf8643e5da32ead7bf2bdd3d0b2ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.5 KB (837537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a7a670a5e4d2d89dcdb42b48576b2715533bce933b3379470a30f2233d03e82`

```dockerfile
```

-	Layers:
	-	`sha256:2967015664fa4db1599501bb4a278e9e5e416e9c5b694ab4fe3c4f2d61a85994`  
		Last Modified: Wed, 13 Dec 2023 04:20:03 GMT  
		Size: 803.6 KB (803639 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5da6fb91cfdd8499f7ab51a5ba718b6958f3077670f58df2908b27e627fbd7a2`  
		Last Modified: Wed, 13 Dec 2023 04:20:03 GMT  
		Size: 33.9 KB (33898 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; 386

```console
$ docker pull postgres@sha256:ab38f3d0b9b27fd9476f65d31f437d0a6b2b42f9859e73a8c4a192fed7999fe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96566191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3442f0e77e4b35ee53405c17d946defbcffa3eeceb1d6fd0d063f72c7baf772`
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
ENV PG_MAJOR=13
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_VERSION=13.12
# Wed, 04 Oct 2023 14:54:45 GMT
ENV PG_SHA256=0da1edcee3514b7bc7ba6dbaf0c00499e8ac1590668e8789c50253a6249f218b
# Wed, 04 Oct 2023 14:54:45 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 04 Oct 2023 14:54:45 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 	echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"postgres-sbom","packages":[{"name":"postgres","versionInfo":"13.12","SPDXID":"SPDXRef-Package--postgres","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/postgres@13.12?os_name=alpine&os_version=3.18"}],"licenseDeclared":"PostgreSQL"}]}' > /usr/local/postgres.spdx.json 	; 	postgres --version # buildkit
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
	-	`sha256:1f98edcbda5d87f134c849bfcf8656230a9dd81f987b9a6bd1d4c72db6e24ba3`  
		Last Modified: Tue, 17 Oct 2023 19:06:00 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de9c05e31f9239e4704d04137ace7b97168544b1df5bd1c3fd7f7a5b6b501e63`  
		Last Modified: Tue, 17 Oct 2023 19:06:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd0a5fcc55d13dbd538afc11793b399296b7355c68c67a6437a33bb44aebbedc`  
		Last Modified: Tue, 17 Oct 2023 19:06:11 GMT  
		Size: 93.3 MB (93314950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3caf44c10069462a74142e22e6c8deaba88bf39d5713151897f51c00ee7d7330`  
		Last Modified: Tue, 17 Oct 2023 19:06:00 GMT  
		Size: 9.0 KB (9020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7113c6593f56dd9faea31456f65b98a116d57f307dac76b6150951faf1b52246`  
		Last Modified: Tue, 17 Oct 2023 19:06:01 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f40011813ba392a5703a0063e2cc7fe7c2c3168b9689b63c59223f6a0d06e979`  
		Last Modified: Tue, 17 Oct 2023 19:06:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb23d5b7ea4c3133b0a458b763bf41b599f926bc7b6a59d7ea574d6c54824eed`  
		Last Modified: Tue, 17 Oct 2023 19:06:01 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:48eb8bdd5818382a74d47253ce0a675230a868455570cc7c1ba8724668be4f69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 KB (35463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:363b276d9831fd99d140c75478d8745d0d62ab2a02e0b9e3cc0d518c1e1636f0`

```dockerfile
```

-	Layers:
	-	`sha256:f769f65b2c0bdc2e6bc5b4a17539a39659e3135bf695602812d0dd977559a032`  
		Last Modified: Tue, 17 Oct 2023 19:06:00 GMT  
		Size: 35.5 KB (35463 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; ppc64le

```console
$ docker pull postgres@sha256:46ca37fef1c69b0745217092543cfbacf9788562cdff17d33e33a124a8178727
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96769192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc843075d2faaa109a960fded506385a27d6b985b9716ecf55f79e3d4e1d75de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bced4bbb414e40d55661e37f75a11c9c92e62c379348aee683b29464d6a543e`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a4a7ebeb5723f2d6edac750fb7416df4bc23bca2d60b598f19901333b484de5`  
		Last Modified: Wed, 13 Dec 2023 03:23:45 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:874421fbe4a200bf7bb8d56cd3a00e1737ee0965baa9febf05fa01f7c1826661`  
		Last Modified: Wed, 13 Dec 2023 03:58:23 GMT  
		Size: 93.4 MB (93405380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8188783ab4e17da318ba5bbe16138c769859a59b245b34fb2043503fb5abb0ba`  
		Last Modified: Wed, 13 Dec 2023 03:58:19 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4a109c1da66dde8b645dec0f706983c8c98e7a334f7d64630221fc084245c1b`  
		Last Modified: Wed, 13 Dec 2023 03:58:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e92b92db807382d0253dec3c2a8f86d8a14f268c65cb79c8c6483e0afc167a`  
		Last Modified: Wed, 13 Dec 2023 03:58:19 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e889d921751147cb000ae62ef0f59a4d4c319caba8a601c8caec2c582162d22d`  
		Last Modified: Wed, 13 Dec 2023 03:58:20 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:35838e5321096a0704e372a94fd8ab8185afe00948a000f45e4eafafcbcd6c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **834.5 KB (834531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed0ced79507c8435bb4916f71b5895a3a2f5d65012090c9f3cd9424d4348895`

```dockerfile
```

-	Layers:
	-	`sha256:56f56c4f8d09402a0f8f4060a508f08f3239577ee624f1da16b49a397c7368c3`  
		Last Modified: Wed, 13 Dec 2023 03:58:20 GMT  
		Size: 800.6 KB (800603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5a9798aaa79218c394c61bc03254fbcc76201f3bfefd8d908bd667c6e782c4e6`  
		Last Modified: Wed, 13 Dec 2023 03:58:19 GMT  
		Size: 33.9 KB (33928 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:c3f985638e0a77b8f517a10a15a8c9e051e10a7c8c11e7d5a5a2dd0cb023d0fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92850567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1394bf3ea9e68df61fd427758364c9b514f08dd2fa3908a8c21854657ba7d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_VERSION=13.13
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Mon, 11 Dec 2023 19:03:58 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 19:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 19:03:58 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 19:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 19:03:58 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 19:03:58 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 19:03:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d9eca7e3578b4c16792649c73fb65141bee2d048a99d88a9450e527a42ff6c9`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6dd2ac5a1eda861bfa4578d408f9e37fb3e11394e1c790c366377d9f15578e1c`  
		Last Modified: Wed, 13 Dec 2023 01:10:51 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7fb9c736d3f340f148e060d24787731f1137efa875c05ecb8653f3ba5428a8a`  
		Last Modified: Wed, 13 Dec 2023 01:35:05 GMT  
		Size: 89.6 MB (89617628 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d290fe735f32d68228731427835ef88169bd12f82c5d02d57343474c879df3ef`  
		Last Modified: Wed, 13 Dec 2023 01:35:04 GMT  
		Size: 9.0 KB (9024 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0ea3d2fc45b4b2474c4b608b76d09d1f9a4d22046d71513df77a88ff8cb6575`  
		Last Modified: Wed, 13 Dec 2023 01:35:04 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc0930c66ae76c4943facb5e5e2b62e96cae7f030e99ad541d2604e4347732bf`  
		Last Modified: Wed, 13 Dec 2023 01:35:04 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fc27e5e30d4bf06c8eb8d1188af21e5ecc91a17abc7a8c913162c53b4231ccc`  
		Last Modified: Wed, 13 Dec 2023 01:35:05 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:12ba6ae9f5660a356c3bece5617bef6a7b186ad0d31e776407aacb7da80abcb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.9 KB (835888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84a7bad5e3c4e6875bdcfd3ffadbb85964f294517ab990c430ad663d0a24fb54`

```dockerfile
```

-	Layers:
	-	`sha256:df73e75ba964213f8cc53a4bac8f989cc3f1e3319c2655dae6b715b0b5e74d15`  
		Last Modified: Wed, 13 Dec 2023 01:35:04 GMT  
		Size: 802.0 KB (801996 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:359f38b4e53ae3ff2707f7ebd7c4805858d8bd81ead72e10fed0b1e59d390a2e`  
		Last Modified: Wed, 13 Dec 2023 01:35:04 GMT  
		Size: 33.9 KB (33892 bytes)  
		MIME: application/vnd.in-toto+json
