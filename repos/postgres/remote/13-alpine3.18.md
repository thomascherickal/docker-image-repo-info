## `postgres:13-alpine3.18`

```console
$ docker pull postgres@sha256:5ff96ad1b7bb4f1c0bb453e5b1f17d091c58cffd1b12a8acf3b95d22d53a461c
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
$ docker pull postgres@sha256:7c2b5b00987ad71846aa04bb885acb0b2593f2b7f25ecf059fa16b6d0156adc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91244945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9dd111a59f127b2bcd27383bfe94d6b6a1f83a98f91d7abf2dd28813fc5ee7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e7c73794aeecd8963856544494e8d1f814590c2ea516448a2ffedd38516bba3`  
		Last Modified: Thu, 14 Dec 2023 18:54:53 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ca78a85f68031f01b86c9bc5859b347c1f921c9ba1932103b05b1d825ce99f2`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e9d00017933d332d7393805946595204853b0572452679b8dc91aa9f5c72bea`  
		Last Modified: Thu, 14 Dec 2023 18:54:55 GMT  
		Size: 87.8 MB (87826298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d3de392a6e57d638b334a6e016510e51599f2c88a855579fa181d71b9bfdb2c`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30d273742c83dad7227d1370c4f6ea4de57f7102aa6b07a54511357ef3e82f51`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96e570c46e671c4282cc623f98e475f90c357d5a046ef945ecf1bbcc553003de`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:257e319339b8c8f9e0cf9a8f9a378d4f62ae3b53c84c3693e52fcab902f2f5fb`  
		Last Modified: Thu, 14 Dec 2023 18:54:55 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93476a93c2d5071ece7b060bdf56f8d9d053e46ec0194f147f92766120149126`  
		Last Modified: Thu, 14 Dec 2023 18:54:55 GMT  
		Size: 184.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:94ddd74ad600c00cde8a5aaf5ce96463371da5be93bdb3783fa33c19d5984a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.3 KB (840264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb6019374d09ff65b656ec0ce9e4e216f6e6f2a4c30a070cb96ea5f9a603069`

```dockerfile
```

-	Layers:
	-	`sha256:dcd478e5ca019d994688a82ed949416f0ea70019aae98dc1a478bc66a82024da`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 803.6 KB (803632 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a13cea098bc3d63b10b7d8d53b3ad130d800d13c10afb9556c06ca434bfc0ca0`  
		Last Modified: Thu, 14 Dec 2023 18:54:54 GMT  
		Size: 36.6 KB (36632 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm variant v6

```console
$ docker pull postgres@sha256:1284c69e1ae40def60946548ad273177eea3d08d55efebd595129a00c74ac00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (89968027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a429dbb617a51e4d1d639e6c75eedcc1cd1c57ad3fda5cd591847bf0adf057ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
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
	-	`sha256:a002b43a904b320952dbf8541effe8b20f6a8bb9ee21b256629116a0d9b2d779`  
		Last Modified: Thu, 14 Dec 2023 18:56:15 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6eae59699216e73bb9efebfd8b5f8b7ebe6fff8788432044b35a87f2baf8be6d`  
		Last Modified: Thu, 14 Dec 2023 18:56:15 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:9de7b6c781a6a1eb7aeabdcb46aa8c2a56a6128eee417e45debdd70c190efd18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 KB (36383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0da6d66516c344b46630dc1130a389970083fff2fcf3614df456709b961bd21`

```dockerfile
```

-	Layers:
	-	`sha256:6b8dc50ba201c5c60bbf08ea971e72a15ad337f188f55e0b4f20105d274683a1`  
		Last Modified: Thu, 14 Dec 2023 18:56:15 GMT  
		Size: 36.4 KB (36383 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm variant v7

```console
$ docker pull postgres@sha256:708de304fca058ffc48c41d505d80d7940736ae40dfbc09619dfab6370cb61e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84672283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e042af0427252c826044c77ed1ecbe190e79981f45f411e5b06aaa7abb898e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
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
	-	`sha256:e801bbb7144dd7e5fdc5bb55208011eb0c7437c18a5b840a00dff7b9336e7a65`  
		Last Modified: Thu, 14 Dec 2023 19:32:10 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:097230f59e1ea4abcfe258d9a5c953679fd0cb6586cd170ced0f784545ab0a0e`  
		Last Modified: Thu, 14 Dec 2023 19:32:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:f94ba67ad5f6936bc62d21714346332c9f3f89e866f37cc1aafa54e7575cd75a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.2 KB (840250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2eaf385fc707dbf0236a0d3a016975fd6b8d1e13f39597fe040d10faa5879e5`

```dockerfile
```

-	Layers:
	-	`sha256:9745885e4b74767a6e0be6bc7d951cb5c48bf7484b7b34df45f2c4d2c6f585b0`  
		Last Modified: Thu, 14 Dec 2023 19:32:11 GMT  
		Size: 803.7 KB (803652 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:85f956a59db60e9e20ba92d28689854bed6032bf09b73f53702fa426cb72a40d`  
		Last Modified: Thu, 14 Dec 2023 19:32:10 GMT  
		Size: 36.6 KB (36598 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:110f41fc68713f2960ba0226748bcd234e2a840ac4553afc47a904e2d842eabe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74db59de8e03c0018d13a49c70b3956204503b75a5d3e1448965865ce783538`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
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
	-	`sha256:57c459ff5a4d2237e0eb9379ce9861cadd8e3b74f3cb1e2ff8c906acf471421a`  
		Last Modified: Thu, 14 Dec 2023 20:28:24 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa33cc4b6885c188b3791ad3ef6008f561d5ffb9a3c9c4d535721a7070693cfa`  
		Last Modified: Thu, 14 Dec 2023 20:28:24 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:7bf646ddbd6aacbb0d5938eadfd2fd7d6081f567cbf388b9f258142f21802814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **840.1 KB (840110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937b0a57da45b1a67b544ead06da3d33036857c03eddb28a1af517bffea59c41`

```dockerfile
```

-	Layers:
	-	`sha256:59cb3b2dfecfb72172de8f1254bad01da1c11cfa9db3eb15d3cb26e5b7f0cced`  
		Last Modified: Thu, 14 Dec 2023 20:28:24 GMT  
		Size: 803.6 KB (803639 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:120a55247862ac10d0cb5d74503f61ce67fbf0e77e0a33b9f3868aa686d0699b`  
		Last Modified: Thu, 14 Dec 2023 20:28:24 GMT  
		Size: 36.5 KB (36471 bytes)  
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
$ docker pull postgres@sha256:711f9cd1d7f2f4fd99c6f736dbb46aaa9d0558f96436e0a1d3bb6b3d64461f53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96769937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf1df4d94e305250b5d79aee5748333bac910dbdbec39b54d8a9bcf7a06c9e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
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
	-	`sha256:7211917eea538178c78e3b464a5cf1b4689456a73131987b945c3f79628a4fea`  
		Last Modified: Thu, 14 Dec 2023 19:26:01 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7efc850b32fde8e3ceded92e6530dc2c158b419c04615b27d8cfb809bb22a1b`  
		Last Modified: Thu, 14 Dec 2023 19:26:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:39494d416dedd6502def7f178f249b1b5cdf23ef4369980be530d59a9ff6fb55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **837.1 KB (837107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98652c7d5cff84ff790099254b57d64fe5a663dce55e34d8817ed0e1a2c6daed`

```dockerfile
```

-	Layers:
	-	`sha256:2787907ed7306b3d586ce87a92ade3fbd7ac5386381809583e5d235207db2cf5`  
		Last Modified: Thu, 14 Dec 2023 19:26:01 GMT  
		Size: 800.6 KB (800603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8e156ab41af1e8d53a98d02b288cefed138864592efc424835f0c790767045e6`  
		Last Modified: Thu, 14 Dec 2023 19:26:01 GMT  
		Size: 36.5 KB (36504 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-alpine3.18` - linux; s390x

```console
$ docker pull postgres@sha256:a89c839383aae8053f141551f2e5ed49367a9b0f013348253b8f1fa228c97e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92851311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb547c2fb422ef55852e3d7b92fc4b58c1739a189c7769b3c22264c84fe2ceb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=13.13
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8af69c2599047a2ad246567d68ec4131aef116954d8c3e469e9789080b37a474
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	cp -v /usr/local/share/postgresql/postgresql.conf.sample /usr/local/share/postgresql/postgresql.conf.sample.orig; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/local/share/postgresql/postgresql.conf.sample # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Dec 2023 22:17:08 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
STOPSIGNAL SIGINT
# Wed, 13 Dec 2023 22:17:08 GMT
EXPOSE map[5432/tcp:{}]
# Wed, 13 Dec 2023 22:17:08 GMT
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
	-	`sha256:f1cbf928c4d328548628041f62661b50a51be817dfd550472ca730b718935904`  
		Last Modified: Thu, 14 Dec 2023 19:16:19 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4651804fc0fd1ea380f8808f175ee894b846940026cfc053e2a0d09df2e3c0b`  
		Last Modified: Thu, 14 Dec 2023 19:16:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-alpine3.18` - unknown; unknown

```console
$ docker pull postgres@sha256:fbe5d634f64ea17ccab8852d1e98d7c6f1a14cf8dfcf5c67ddb03d0f52a517c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **838.5 KB (838462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e1021ccf6ee7c5a36d9aef2e37c8432a230de5f51056644b4fdaeb39afe98a`

```dockerfile
```

-	Layers:
	-	`sha256:fd1148651a6b4e52fa73e428c066e214294380df79b695961db617e5c50d0870`  
		Last Modified: Thu, 14 Dec 2023 19:16:20 GMT  
		Size: 802.0 KB (801996 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:00275fc5e7aabcaf5670536415aa3c77871975311f84e1bb5652b4a8d136a0bc`  
		Last Modified: Thu, 14 Dec 2023 19:16:19 GMT  
		Size: 36.5 KB (36466 bytes)  
		MIME: application/vnd.in-toto+json
