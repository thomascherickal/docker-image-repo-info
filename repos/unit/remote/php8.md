## `unit:php8`

```console
$ docker pull unit@sha256:2cfce1e4dbd12ecf625132d01d141e1f82d4fa7742b5b4e15f7d766496f71971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `unit:php8` - linux; amd64

```console
$ docker pull unit@sha256:f107545443e98fdd3a7de495ee1792926a8e8714866a09de0cabfc9a12520303
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189473268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49f1448f418ed9c16af10fc28a8f0754dff1da5e55f3fa27157cc3a10e73def`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:23 GMT
ADD file:4a063d4e089ef10c6806d7042a0040078674ac2db61df02df8bbb8fa4894910a in / 
# Tue, 04 Jul 2023 01:20:23 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 13:39:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 13:39:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 13:40:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:40:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 13:40:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 13:40:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 13:40:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 13:40:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 14:08:58 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 10 Jul 2023 22:05:15 GMT
ENV PHP_VERSION=8.2.8
# Mon, 10 Jul 2023 22:05:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Mon, 10 Jul 2023 22:05:16 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Mon, 10 Jul 2023 22:05:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 10 Jul 2023 22:05:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:08:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 22:08:27 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Mon, 10 Jul 2023 22:08:27 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 22:08:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 22:08:27 GMT
CMD ["php" "-a"]
# Tue, 11 Jul 2023 00:03:42 GMT
LABEL org.opencontainers.image.title=Unit
# Tue, 11 Jul 2023 00:03:42 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 11 Jul 2023 00:03:42 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 11 Jul 2023 00:03:43 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 11 Jul 2023 00:03:43 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 11 Jul 2023 00:03:43 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 11 Jul 2023 00:03:43 GMT
LABEL org.opencontainers.image.version=1.30.0
# Tue, 11 Jul 2023 00:04:41 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && hg clone -u 1.30.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --pid=/var/run/unit.pid                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 11 Jul 2023 00:04:41 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 11 Jul 2023 00:04:41 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 11 Jul 2023 00:04:41 GMT
STOPSIGNAL SIGTERM
# Tue, 11 Jul 2023 00:04:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 11 Jul 2023 00:04:41 GMT
EXPOSE 80
# Tue, 11 Jul 2023 00:04:42 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:9d21b12d5fab9ab82969054d72411ce627c209257df64b6057016c981e163c30`  
		Last Modified: Tue, 04 Jul 2023 01:25:43 GMT  
		Size: 31.4 MB (31417388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2f438b30581593b3d4296a477ca4f824e7d5d680b7e34281e3a3d309ce7f28`  
		Last Modified: Tue, 04 Jul 2023 16:17:15 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04ed8a9ea49fbc2a12ed1b0d62952138c95ae060eaa94a8a8e71469eb6d4424`  
		Last Modified: Tue, 04 Jul 2023 16:17:26 GMT  
		Size: 91.6 MB (91635583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10478cdfe5dae28f47467d50b3247339d7d7dcda74203fe83b5be38ab63603e3`  
		Last Modified: Tue, 04 Jul 2023 16:17:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275da7b7714915d0d85690b691b6fcf97362cbe77df56a08779a804ce0cef48`  
		Last Modified: Mon, 10 Jul 2023 23:51:38 GMT  
		Size: 12.4 MB (12354515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e00a9b8328b3a0d9e1f53bcc8ee0aeaee02fdefc84bf8371511c13727e5929`  
		Last Modified: Mon, 10 Jul 2023 23:51:37 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c4232fbd2f59aaff54f06698599ffd9798d4824a5ce00afb08d8013a74926c`  
		Last Modified: Mon, 10 Jul 2023 23:51:42 GMT  
		Size: 34.6 MB (34557669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37880c6b41d522f374721252526e821fe80bb686a64e834c3fe31d8f5c3a0601`  
		Last Modified: Mon, 10 Jul 2023 23:51:38 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4cdae91cfd746ee40da98e721afcc2a9e76115093ef321cff21891cf5f4b619`  
		Last Modified: Mon, 10 Jul 2023 23:51:37 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d8e3940c7a6728419bf7ad9d0cc5dba585a0f7f908931c0520edda9711164`  
		Last Modified: Tue, 11 Jul 2023 00:05:30 GMT  
		Size: 19.5 MB (19501709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800051601c771c1a1b9c8ec2b5e49cb078845e2648200c673867c9303a7810c9`  
		Last Modified: Tue, 11 Jul 2023 00:05:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b665403708eea6ebc21650b354d6fc345fd27af3db3dabf3febadd540c109f15`  
		Last Modified: Tue, 11 Jul 2023 00:05:27 GMT  
		Size: 1.5 KB (1463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `unit:php8` - linux; arm64 variant v8

```console
$ docker pull unit@sha256:2eb86106a9ff94c1c08617cf9d0418ede0b50857497b7d49058fbc5c6ecb9fea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.2 MB (183182411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88f93ce08ebe5f80f282d060a86cbf18a1154bf51b8da2f0aa7545aaabce6b07`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["unitd","--no-daemon","--control","unix:\/var\/run\/control.unit.sock"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:52 GMT
ADD file:83a81aad5cdb80c654a520d913c8bcafe2b8e1062d81c389d4577cde5ad68167 in / 
# Tue, 04 Jul 2023 01:57:52 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:09:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Jul 2023 10:09:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Jul 2023 10:09:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:09:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Jul 2023 10:09:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 04 Jul 2023 10:09:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:09:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Jul 2023 10:09:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Jul 2023 10:36:56 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 04 Jul 2023 11:03:07 GMT
ENV PHP_VERSION=8.2.7
# Tue, 04 Jul 2023 11:03:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Tue, 04 Jul 2023 11:03:07 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Tue, 04 Jul 2023 11:03:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Jul 2023 11:03:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Jul 2023 11:06:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--enable-embed 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 04 Jul 2023 11:06:05 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 04 Jul 2023 11:06:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Jul 2023 11:06:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Jul 2023 11:06:05 GMT
CMD ["php" "-a"]
# Tue, 04 Jul 2023 16:55:09 GMT
LABEL org.opencontainers.image.title=Unit
# Tue, 04 Jul 2023 16:55:09 GMT
LABEL org.opencontainers.image.description=Official build of Unit for Docker.
# Tue, 04 Jul 2023 16:55:09 GMT
LABEL org.opencontainers.image.url=https://unit.nginx.org
# Tue, 04 Jul 2023 16:55:09 GMT
LABEL org.opencontainers.image.source=https://github.com/nginx/unit
# Tue, 04 Jul 2023 16:55:10 GMT
LABEL org.opencontainers.image.documentation=https://unit.nginx.org/installation/#docker-images
# Tue, 04 Jul 2023 16:55:10 GMT
LABEL org.opencontainers.image.vendor=NGINX Docker Maintainers <docker-maint@nginx.com>
# Tue, 04 Jul 2023 16:55:10 GMT
LABEL org.opencontainers.image.version=1.30.0
# Tue, 04 Jul 2023 16:55:57 GMT
RUN set -ex     && savedAptMark="$(apt-mark showmanual)"     && apt-get update     && apt-get install --no-install-recommends --no-install-suggests -y ca-certificates mercurial build-essential libssl-dev libpcre2-dev curl pkg-config     && mkdir -p /usr/lib/unit/modules /usr/lib/unit/debug-modules     && hg clone -u 1.30.0-1 https://hg.nginx.org/unit     && cd unit     && NCPU="$(getconf _NPROCESSORS_ONLN)"     && DEB_HOST_MULTIARCH="$(dpkg-architecture -q DEB_HOST_MULTIARCH)"     && CC_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_CFLAGS_MAINT_APPEND="-Wp,-D_FORTIFY_SOURCE=2 -fPIC" dpkg-buildflags --get CFLAGS)"     && LD_OPT="$(DEB_BUILD_MAINT_OPTIONS="hardening=+all,-pie" DEB_LDFLAGS_MAINT_APPEND="-Wl,--as-needed -pie" dpkg-buildflags --get LDFLAGS)"     && CONFIGURE_ARGS_MODULES="--prefix=/usr                 --statedir=/var/lib/unit                 --control=unix:/var/run/control.unit.sock                 --pid=/var/run/unit.pid                 --log=/var/log/unit.log                 --tmpdir=/var/tmp                 --user=unit                 --group=unit                 --openssl                 --libdir=/usr/lib/$DEB_HOST_MULTIARCH"     && CONFIGURE_ARGS="$CONFIGURE_ARGS_MODULES                 --njs"     && make -j $NCPU -C pkg/contrib .njs     && export PKG_CONFIG_PATH=$(pwd)/pkg/contrib/njs/build     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd-debug     && make clean     && ./configure $CONFIGURE_ARGS --cc-opt="$CC_OPT" --ld-opt="$LD_OPT" --modulesdir=/usr/lib/unit/modules     && make -j $NCPU unitd     && install -pm755 build/sbin/unitd /usr/sbin/unitd     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/debug-modules --debug     && ./configure php     && make -j $NCPU php-install     && make clean     && ./configure $CONFIGURE_ARGS_MODULES --cc-opt="$CC_OPT" --modulesdir=/usr/lib/unit/modules     && ./configure php     && make -j $NCPU php-install     && cd     && rm -rf unit     && for f in /usr/sbin/unitd /usr/lib/unit/modules/*.unit.so; do         ldd $f | awk '/=>/{print $(NF-1)}' | while read n; do dpkg-query -S $n; done | sed 's/^\([^:]\+\):.*$/\1/' | sort | uniq >> /requirements.apt;        done     && apt-mark showmanual | xargs apt-mark auto > /dev/null     && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; }     && ldconfig     && mkdir -p /var/lib/unit/     && mkdir /docker-entrypoint.d/     && groupadd --gid 999 unit     && useradd          --uid 999          --gid unit          --no-create-home          --home /nonexistent          --comment "unit user"          --shell /bin/false          unit     && apt-get update     && apt-get --no-install-recommends --no-install-suggests -y install curl $(cat /requirements.apt)     && apt-get purge -y --auto-remove     && rm -rf /var/lib/apt/lists/*     && rm -f /requirements.apt     && ln -sf /dev/stdout /var/log/unit.log
# Tue, 04 Jul 2023 16:55:57 GMT
COPY file:8b65557c2137d1a3946148e09ddd45af0b855e40210dabb5a9bd6c36fac22006 in /usr/local/bin/ 
# Tue, 04 Jul 2023 16:55:58 GMT
COPY multi:0ef77957b92a7e8997661453cf7256a81db39d0e9f975a137d7e664007d8fcf4 in /usr/share/unit/welcome/ 
# Tue, 04 Jul 2023 16:55:58 GMT
STOPSIGNAL SIGTERM
# Tue, 04 Jul 2023 16:55:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 16:55:58 GMT
EXPOSE 80
# Tue, 04 Jul 2023 16:55:58 GMT
CMD ["unitd" "--no-daemon" "--control" "unix:/var/run/control.unit.sock"]
```

-	Layers:
	-	`sha256:50eb042e2421869704212f3e076e9088033eb9a5254341fb1b3022e6e2784921`  
		Last Modified: Tue, 04 Jul 2023 02:02:00 GMT  
		Size: 30.1 MB (30062957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c3328f3ce997e7bc0f2b47ad766b6c760dd65095a9c1ad9090e66d25a90c09`  
		Last Modified: Tue, 04 Jul 2023 12:30:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30726b692873954b2e0584bc53be8a051244a3d0cfb76833bd6b2915f61e1588`  
		Last Modified: Tue, 04 Jul 2023 12:30:39 GMT  
		Size: 86.9 MB (86928257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cfdeca8ab9e389a7c0e5b3a7cb7c02e9bd2fdf2a147dc8728c81065865a1f2`  
		Last Modified: Tue, 04 Jul 2023 12:30:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf302e3f5bd20010bae5f1cb54ca3c16dadc7eca9e67661c42958243c1f515e`  
		Last Modified: Tue, 04 Jul 2023 12:35:46 GMT  
		Size: 12.3 MB (12336081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72a79c59e9435c3c1d0379fc01eafa86586909e17e00ecc08443df052d921e`  
		Last Modified: Tue, 04 Jul 2023 12:35:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c344e7bb8104180b9916a30d355bd30866a358883179efc651f6352f0aca8da0`  
		Last Modified: Tue, 04 Jul 2023 12:35:50 GMT  
		Size: 34.5 MB (34473709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6b60e63cc1987b69e167d10908e785d287a8013364ee438ce7abb60367c286`  
		Last Modified: Tue, 04 Jul 2023 12:35:46 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d577b671f3329a50cc4f17a34233103a65b36648a29fe7a4dd5e329bb16d0fb2`  
		Last Modified: Tue, 04 Jul 2023 12:35:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59253a33bac5180e18c7e2f6246af6c0a489e29fc826c09677abf83ceb9dbbd4`  
		Last Modified: Tue, 04 Jul 2023 16:57:49 GMT  
		Size: 19.4 MB (19374999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da40c218d508e956ed35729b788e30c743ff4e225b847f04b65594c0326e624`  
		Last Modified: Tue, 04 Jul 2023 16:57:46 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc6253fd53fce95788a45cd5dd853e84883671c5bedd0eeb341214678cdf5bf`  
		Last Modified: Tue, 04 Jul 2023 16:57:47 GMT  
		Size: 1.5 KB (1462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
