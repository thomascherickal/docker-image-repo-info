## `postgres:15-alpine3.19`

```console
$ docker pull postgres@sha256:986d149cfbbb0c818d18e351d3dba2d77ff6f54e045eff5e8dfdc7f82e143c77
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 12
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `postgres:15-alpine3.19` - linux; amd64

```console
$ docker pull postgres@sha256:5a478cbc7036d3ee788060b1a1a55701522b00ab6099b6c368b50f35859f8641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94820690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94362bdb5ee73453450da5fa11c09dfb15ade794164b7c3f911aeac207759ac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4a3f96ea8e50112b86a5f7298e2981a99a4c4b47994cf9ffc722e878d1e8d66`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c1e2e159ea1c71a0352fc365e56bc6a9dccde6d41073aaab2b6d151863c8d8e`  
		Last Modified: Thu, 14 Dec 2023 18:51:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26c071a8426e34b10393f87a034bbbb51ce7c2ce0fe1d20e62924027d16f6bf8`  
		Last Modified: Thu, 14 Dec 2023 18:55:25 GMT  
		Size: 91.4 MB (91395569 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9a1ba05d22ce7880bba072d67f3a1b5f4511af98bbd1076da3e003e9bb580e0`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 9.4 KB (9443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efc39a79d7dc32573b6e891a1b930d00b1cd6ccb7f38eff69f1d5670be80dc2a`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72124e665f9e4ee541e264d27549f7dde1aeb600a7f84b3277458239f2a27e10`  
		Last Modified: Thu, 14 Dec 2023 18:55:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa569f3e770ef0233bf5e7f1b25d4a3a9bfa731076c0fb3b342e33890daa6004`  
		Last Modified: Thu, 14 Dec 2023 18:55:24 GMT  
		Size: 5.3 KB (5337 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86d5fe07cb374a1d2214c8f055ce22000263c237c22321a269abee687be4b8e7`  
		Last Modified: Thu, 14 Dec 2023 18:55:24 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:f48e4d1c6928f8dca68d48c52b9a7e662b269d1172d85e8eaa794c5ed9f55533
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **845.2 KB (845156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e967aecc90c56b7bf3ab3e9dfc31d829ed7f95f018296956829afbeb50da1b`

```dockerfile
```

-	Layers:
	-	`sha256:4a1400e3169f3aa5e87cd33939da378d1bbef707351bc43f4b450d75807b2df8`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 807.3 KB (807311 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c2b0b3b2c3df020097d5cfaf161ed16bf2e06cf26efc24ccd44c576503c3a24c`  
		Last Modified: Thu, 14 Dec 2023 18:55:23 GMT  
		Size: 37.8 KB (37845 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-alpine3.19` - linux; arm variant v6

```console
$ docker pull postgres@sha256:bccd09bff2c1928024359e270f02e842f6923a966646642263d1ddfe581a4e73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.6 MB (93595631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17518bfaf745ac980409d119cb15d7f67e4b43c1c70e88022e195aa65bbca817`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93216e21790982df0e80b11285a7034d070a4c27658e9293911a2366ccc04d0f`  
		Last Modified: Tue, 12 Dec 2023 22:34:35 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01f971838734b144cc183181c1a5434902d7407a183c836ec25e35654d41ad57`  
		Last Modified: Tue, 12 Dec 2023 22:34:35 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:656b73bceae6e7acdf4f720628a04e7461bec0aa77696277806268ff3919d8af`  
		Last Modified: Tue, 12 Dec 2023 23:36:06 GMT  
		Size: 90.4 MB (90413830 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:066de59f0e9aee820ce700e85ef2ed423d4c13fb0cbf110aaa9537be7d146802`  
		Last Modified: Tue, 12 Dec 2023 23:36:02 GMT  
		Size: 9.4 KB (9449 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7483ec50e7e34e64b9c5de785067f630f8ea6d8abedde7bca54fabe2f82a622b`  
		Last Modified: Tue, 12 Dec 2023 23:36:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91162ace8c0bc1af3dec62f0fbf730710c21d18675c9ed90c38fa4a16b728f3e`  
		Last Modified: Tue, 12 Dec 2023 23:36:02 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd6bd71211695355f8252a6e435fbafa6ad8bdba181a11a2205f18c1e9faadcc`  
		Last Modified: Thu, 14 Dec 2023 18:54:51 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f407f0067481b508cb9e3219fe6ebde29befe943d4c462e3c3e5203e6ff7b52d`  
		Last Modified: Thu, 14 Dec 2023 18:54:51 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:73da69fe943cdfd86bbe1b9a6e1335a6542b435a676886bd5fe513f4544336ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 KB (37612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296dbc06846861a672dbed22891a5e10057dfd2dec039560e09d031805f08407`

```dockerfile
```

-	Layers:
	-	`sha256:5b585396b9348ec0b3227b4682b627d6d0530f03ac8a4299dd48ce8f40e0d08e`  
		Last Modified: Thu, 14 Dec 2023 18:54:51 GMT  
		Size: 37.6 KB (37612 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-alpine3.19` - linux; arm variant v7

```console
$ docker pull postgres@sha256:fa6d3fd0b19ccfe2909748d9401dd3e56de79a3af0c6ac6330f16aba0e415ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (88048852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac17ee4c5f72dac4d8039e1adc087b79eba1ebbdc7431add43fa6c361b018a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27ced7217800ddaf8587a82f36031cc326f5fad72be92ddaf3190274dfaf9349`  
		Last Modified: Sat, 09 Dec 2023 05:56:24 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:775f31fd0943cf8717d7b087da7493680a94ea12d1b324c7a9a10aa97815a8d9`  
		Last Modified: Sat, 09 Dec 2023 05:56:24 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7af862696551ae2c5ad29774ef38ab3278c989452ef35136f0abb23548e11a0`  
		Last Modified: Wed, 13 Dec 2023 02:00:05 GMT  
		Size: 85.1 MB (85113499 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e34a0c337c2d14358e45cdc44f5a5585e98653f10016bfb0d38992260eff5337`  
		Last Modified: Wed, 13 Dec 2023 02:00:02 GMT  
		Size: 9.4 KB (9449 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36ca49293cfa401896e39bfb6125ad316b9e84dc97e7fce9971cab8fd5be5a01`  
		Last Modified: Wed, 13 Dec 2023 02:00:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a22167ea71e9739225c66e96e28c1b97bc4b45d108f09c9b4e527f60016ee223`  
		Last Modified: Wed, 13 Dec 2023 02:00:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85583903bea66acbfa32ee34c2369282a4d807d02139e0f5368a8e939e822864`  
		Last Modified: Thu, 14 Dec 2023 19:28:15 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcd010e8b45cd524eb1297b62124ae128b9c9132bbdb19b34fd4d69007ed870b`  
		Last Modified: Thu, 14 Dec 2023 19:28:15 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:abe9faa0bd710268abc03e7aa0619ced01e425159a0cf2a5bb731394e0824f62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **845.2 KB (845174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a69ded8ec0755893ab21b9dfa8c562c256206a0e165698a1352cec08a29e0f`

```dockerfile
```

-	Layers:
	-	`sha256:194821b1761d4fdea3ba7afb57f28192684bdb45eb4d55c69bdfb72a7e061c1a`  
		Last Modified: Thu, 14 Dec 2023 19:28:16 GMT  
		Size: 807.3 KB (807347 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1511ebff6ec70401955c74ada1a9d201a088adc4b864841cec30ffe01ba2393e`  
		Last Modified: Thu, 14 Dec 2023 19:28:15 GMT  
		Size: 37.8 KB (37827 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-alpine3.19` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4bd6b94e226f293ffdb1c556e7d9e3f7a191cc3bb69c847012722229480d052c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.6 MB (93588016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41cdd6fe6b0c08fcf3026b8b78843a1c2ae34c28ffc20264134cef5c5e27dc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20a13ecc88456148cc73b8941875af2463232293d6e48313a5d057f52f188e04`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01277bc8c6d336069acfe7e4b99842b4e64eb3c6b65bd1dd31d3a6a8a1d98b16`  
		Last Modified: Wed, 13 Dec 2023 02:39:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eee02989f6306e22575ae35b0f07fc29d52c4ac074afa51b91c0608509cab2b`  
		Last Modified: Wed, 13 Dec 2023 03:40:14 GMT  
		Size: 90.2 MB (90223569 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ead3ef10950588847b35c2422f2e79430c9c30618f23ccf898c1beabaa89934`  
		Last Modified: Wed, 13 Dec 2023 03:40:11 GMT  
		Size: 9.4 KB (9448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f27916a8624f2c01c9cc2fab3cdab404f776562bf917d405c50ae4cf33211ebc`  
		Last Modified: Wed, 13 Dec 2023 03:40:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d1130d561c76a7c6e598d18a45b0e4442930468989963b093945b788600f9ac`  
		Last Modified: Wed, 13 Dec 2023 03:40:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53af004835e3fbb088e73070e4545b0b6774dee44732c7c3530528f47f59de1a`  
		Last Modified: Thu, 14 Dec 2023 20:22:39 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c31d30d83c8edfa59002ffa86412a7adce40bcb4d37f3b91d91c3184484aa46c`  
		Last Modified: Thu, 14 Dec 2023 20:22:39 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:4c8cb46d1944bc006f6ac2afba32d9031f6a878d637a8c5c64a7dcf277637fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **845.0 KB (845011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5facb318ef6e36c8c93def072b77cb79f875f69fe0e0bf67ceb006e0add203a2`

```dockerfile
```

-	Layers:
	-	`sha256:5500db4b14aca0f015500f9e33298831cfcc4c65dab8f6469fc694deb0af648e`  
		Last Modified: Thu, 14 Dec 2023 20:22:39 GMT  
		Size: 807.3 KB (807322 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0fb45b382a6ea145f826dd09fcc2d6a414efb121442fa9cd3f2ed877a1bd99fb`  
		Last Modified: Thu, 14 Dec 2023 20:22:39 GMT  
		Size: 37.7 KB (37689 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-alpine3.19` - linux; ppc64le

```console
$ docker pull postgres@sha256:a25b2511fe4f45a5d38200af7ea93fadeebf2cb6185e4088297fb2f8da42f0f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99432272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5dc6744d1fdfb1d706588e85612b5a5803d9e2e1cc71e174d1b44f673b1c007`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:d9fd01bd45787259e329462915a9f7da214e8b4a6f5f93d8af167e299526ee74`  
		Last Modified: Wed, 13 Dec 2023 03:34:24 GMT  
		Size: 96.1 MB (96057381 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:441955daf58166a2126a58d25f448b2186db745ab8bf77f9927d881f54d5bf09`  
		Last Modified: Wed, 13 Dec 2023 03:34:21 GMT  
		Size: 9.5 KB (9453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f08b8ddeb7e5d4321d8914e2c74026ddfcafa4dc2d7f19ede7dbb5d57f41b161`  
		Last Modified: Wed, 13 Dec 2023 03:34:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e592e192ab8bb51c1a33f6d763675d5b6977019b8a937bcf764cd7d773bc338d`  
		Last Modified: Wed, 13 Dec 2023 03:34:21 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b59168de4ff9bdb0e6a6c69f8ea69047d9db199b0ec63face67d5d9df8d7841`  
		Last Modified: Thu, 14 Dec 2023 19:19:31 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67c8086798cf57ffd3785773cbdbb76712ce6a0dc9e489144732454559e605ab`  
		Last Modified: Thu, 14 Dec 2023 19:19:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:9dc9faa845f5ffa64443708d7c4e56830677e98c1cad03852665bc566b2fec76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **842.0 KB (842023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1bb605fca4cbfc74a7faf19f5a32421a21b6a11287552304e251b453bd03e78`

```dockerfile
```

-	Layers:
	-	`sha256:eb05f6465e6255fb4412c163ba937e5e4bbc5dd920158886de509c7a0ce7d887`  
		Last Modified: Thu, 14 Dec 2023 19:19:31 GMT  
		Size: 804.3 KB (804294 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b4b8f8106087d1387457bc3a53bad0133cba3e0cc7d5a38d7517e496d88b98f9`  
		Last Modified: Thu, 14 Dec 2023 19:19:31 GMT  
		Size: 37.7 KB (37729 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-alpine3.19` - linux; s390x

```console
$ docker pull postgres@sha256:349afcc9d53401e6c554b8231dcf9baed0265db34a564cfe3cc4c13d8c511c3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103732869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dad1023e27a5281f5c649933fd7e10876f501d20f30a80c25677f8d74f0863b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV LANG=en_US.utf8
# Wed, 13 Dec 2023 22:17:08 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_MAJOR=15
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_VERSION=15.5
# Wed, 13 Dec 2023 22:17:08 GMT
ENV PG_SHA256=8f53aa95d78eb8e82536ea46b68187793b42bba3b4f65aa342f540b23c9b10a6
# Wed, 13 Dec 2023 22:17:08 GMT
ENV DOCKER_PG_LLVM_DEPS=llvm15-dev 		clang15
# Wed, 13 Dec 2023 22:17:08 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		$DOCKER_PG_LLVM_DEPS 		bison 		coreutils 		dpkg-dev dpkg 		flex 		g++ 		gcc 		krb5-dev 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openldap-dev 		openssl-dev 		perl-dev 		perl-ipc-run 		perl-utils 		python3-dev 		tcl-dev 		util-linux-dev 		zlib-dev 		icu-dev 		lz4-dev 		zstd-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 		export LLVM_CONFIG="/usr/lib/llvm15/bin/llvm-config"; 	export CLANG=clang-15; 		./configure 		--enable-option-checking=fatal 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 		--with-gssapi 		--with-ldap 		--with-tcl 		--with-perl 		--with-python 		--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 		--with-lz4 		--with-zstd 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 			| grep -v -e perl -e python -e tcl 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 		zstd 		icu-data-full 		$([ "$(apk --print-arch)" != 'ppc64le' ] && echo 'nss_wrapper') 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version # buildkit
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
	-	`sha256:08fe0d0e9797a7cadebcb9f89807585a8c515935583ddf26492f628af7fe8895`  
		Last Modified: Wed, 13 Dec 2023 01:15:57 GMT  
		Size: 100.5 MB (100473881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6a4ba2dbde456e7e1b214ec36f688b360e4d1754406d854dc8344aa400cbaf5`  
		Last Modified: Wed, 13 Dec 2023 01:15:55 GMT  
		Size: 9.4 KB (9448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:318f140a774fb16573a981e18430b2007857436e11283aa23b78cbf8515876de`  
		Last Modified: Wed, 13 Dec 2023 01:15:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1bf82eb4fc3e196e78278e3254263e09fd9d73c5b6e9e8b8d29b412e42078ec`  
		Last Modified: Wed, 13 Dec 2023 01:15:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00b6925f4baba2aab020f3f52fd8f815fc55cce157236c72b6aaea0f4f40d690`  
		Last Modified: Thu, 14 Dec 2023 19:11:18 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85d28bdc42b888ed39528cb1f3db69bd76f9698a970c6b8fb2d65fb14e633b8f`  
		Last Modified: Thu, 14 Dec 2023 19:11:18 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-alpine3.19` - unknown; unknown

```console
$ docker pull postgres@sha256:3704642d232b5867a6d439eb776a8697dea40a86ecafdb3fb7268b9fabef15d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **843.4 KB (843360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9493b6681472063969894032dd80b441f6fd5a5b6db0d87ba9bc82916d8c51ac`

```dockerfile
```

-	Layers:
	-	`sha256:37eb75912c59ae459fb3e7764feea41ac758a27a41a1fed7882e14052077dca8`  
		Last Modified: Thu, 14 Dec 2023 19:11:17 GMT  
		Size: 805.7 KB (805675 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:841babb36da6ebc78e66fe39f027543d3fa2dbf698a1c208bb91f50bf7ceb086`  
		Last Modified: Thu, 14 Dec 2023 19:11:17 GMT  
		Size: 37.7 KB (37685 bytes)  
		MIME: application/vnd.in-toto+json
