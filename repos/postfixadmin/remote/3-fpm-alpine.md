## `postfixadmin:3-fpm-alpine`

```console
$ docker pull postfixadmin@sha256:86b62032a301a88c1a1f4a6c0e99a32652ec6df0d101fa6c269ba3e880c466dd
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

### `postfixadmin:3-fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:d15f7912cda6372c2a2a4c09b041bb85c566f23f14499ffaee46b8f84b02791b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35332323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dc1c8e9b49df133a190881a6792f2fa6666752e63cd803a7851ecae83ee5c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:39:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:39:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:39:10 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:39:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:51:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:51:18 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:51:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:51:18 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:51:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:58:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:58:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:58:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:58:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:58:48 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:58:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:58:48 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:58:49 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:58:49 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 23:23:53 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 23:23:54 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 23:24:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 00:55:19 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 00:55:19 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 00:55:19 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 00:55:19 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 00:55:20 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 00:55:20 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 00:55:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 00:55:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b6029f6920d234861e6cee7ca87a1840de19c6049c86038f1fb9432e32ea6d`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 1.9 MB (1864199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55761811b31b62dd8f7c87e712cac077dacc6a20312b0e2a382c9bdb8315777c`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750fd99fe831a06b99ef6e82d1c1be04f9bf478c24ea2d52d63ac918c90df13`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005fd6a0b1925cb2a3f89ec9e421e1c8834862adc32b069b7b90498c4714cae1`  
		Last Modified: Wed, 30 Nov 2022 22:07:38 GMT  
		Size: 11.8 MB (11822991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb649c32f4789c903e8da83afe9718242913abf762d10ba569275708680c994`  
		Last Modified: Wed, 30 Nov 2022 22:07:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4291161e70f2a98a22fa81e7c7a74b5ebafe82bafd66abbb24b904fd2c6142f`  
		Last Modified: Wed, 30 Nov 2022 22:08:20 GMT  
		Size: 12.5 MB (12473521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b8f7e26c455aab3cf850f1b8fcc2035bf7c782e6c6891fbb451dcf6ac7065`  
		Last Modified: Wed, 30 Nov 2022 22:08:18 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3555631404995bc00b9bd633f95d624f08dafdbb34b54e339f3663911f6b1a9b`  
		Last Modified: Wed, 30 Nov 2022 22:08:18 GMT  
		Size: 19.0 KB (18951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4920702e1170004e6bdb5cd0b47ec0fc34793bb5f6affd676af9a34967e644`  
		Last Modified: Wed, 30 Nov 2022 22:08:19 GMT  
		Size: 8.6 KB (8620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157153caa7054ebf9b304486d89c723ff4667fc11bdcb94ad36ddec597240588`  
		Last Modified: Thu, 01 Dec 2022 23:25:31 GMT  
		Size: 501.2 KB (501213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1570e0be126152f85aefb828e8acd799d71899766e20205591452429cbf10fe`  
		Last Modified: Thu, 01 Dec 2022 23:25:31 GMT  
		Size: 3.4 MB (3403191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86170bf61cdff700b6f78e90ffd2d583d15a1effe02e6468d76da5a74f906319`  
		Last Modified: Fri, 09 Dec 2022 00:56:21 GMT  
		Size: 1.9 MB (1862855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a39820af05a74c1ced1f0fbcdeecaf62bea634786092445fad840e57a458be`  
		Last Modified: Fri, 09 Dec 2022 00:56:21 GMT  
		Size: 1.6 KB (1602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:c07c79758d002e22986660f4c9050611c3d59247e66d195fea2f2af17a29476f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33468816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b4653fb4adf701f169b20e436aded3e01e35a33a18be425bd5924857f297b3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:31:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:31:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:31:03 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:31:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:31:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:43:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:43:49 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:43:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:43:49 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:43:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:43:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:51:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:51:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:51:38 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:51:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:51:38 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:51:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:51:38 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:51:39 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:51:39 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 22:49:36 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 22:49:37 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 22:50:15 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 01:01:20 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:01:21 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:01:21 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:01:21 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:01:23 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 01:01:23 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 01:01:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 01:01:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519fe767bb0c7928a1dbb3eed5885ac27b686566653a40e08b8377c7efeb5965`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 1.8 MB (1848421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d73d4fd50e3aae901afb655f4fb90048c5f350001b4d52bb8d1bc50424c93a`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c342b7908a6480c9e4c98966c37148ce29d0f29d1ceabe2775acbbf4e4dd0698`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3e5211bb7f92bcda9884ce9b6b564f4185660332d7d6b1e7f929e06d5087de`  
		Last Modified: Wed, 30 Nov 2022 22:02:00 GMT  
		Size: 11.8 MB (11822957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe86b0e4c6956ccb6274d39239f93b97cc7ff2442c7bed4cb5e3289c692df60e`  
		Last Modified: Wed, 30 Nov 2022 22:01:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb33ef97547bb41569a69b29bac6528889ec8cd5f5820517360fc78e7e48aabc`  
		Last Modified: Wed, 30 Nov 2022 22:03:03 GMT  
		Size: 11.3 MB (11277098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abcd2a2ab28b3e61d2e5ee8f0113a8d4ee30c1c769b5f8047d544af8e59a57e`  
		Last Modified: Wed, 30 Nov 2022 22:02:59 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd65899ef2d2c552e7c3dd0bbf15f53bb9c8accd7aab934ad81c69c108f29a81`  
		Last Modified: Wed, 30 Nov 2022 22:03:00 GMT  
		Size: 18.7 KB (18715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dedbd9e4fefe3ef3dff6adf15d726dde3f6a774cf03222e40355a14a7617d36`  
		Last Modified: Wed, 30 Nov 2022 22:03:00 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa5ce072a78e2b925dacea0075525096d839627309b57a63dbd7d7d63676338`  
		Last Modified: Thu, 01 Dec 2022 22:50:42 GMT  
		Size: 527.5 KB (527542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345a2104ca561e06a827cc87d614d6dbc5cd4c3ccf694a2220fce24ef0cb1dff`  
		Last Modified: Thu, 01 Dec 2022 22:50:42 GMT  
		Size: 3.0 MB (2989519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ea22c8c1c99fb7c9fbec4bbf0b40505ad1fe15ca23d8542801537082c7d9c`  
		Last Modified: Fri, 09 Dec 2022 01:01:44 GMT  
		Size: 1.9 MB (1862808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8990b730adce1ee0c93ad0242182f8b47ec2ab3c283370230e4cef0bf26db0f4`  
		Last Modified: Fri, 09 Dec 2022 01:01:43 GMT  
		Size: 1.6 KB (1600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:c17837b6e96f0435bd33c8579ee5d039ef72834f51415cd8ffb7dbc5a1b3aac0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32591234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e350f8b607792bd8cc0dd0db76b6b72743741d069cdb3db2335d6d02069b12b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:47:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:47:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:47:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:47:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 22:01:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 22:01:28 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 22:01:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 22:01:28 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 22:01:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 22:01:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 22:07:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 22:07:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 22:07:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 22:07:45 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 22:07:45 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 22:07:46 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 22:59:38 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 22:59:40 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 23:00:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 00:58:22 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 00:58:22 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 00:58:22 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 00:58:22 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 00:58:23 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 00:58:24 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 00:58:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 00:58:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca108fdbcd11a67cf41e6ad58105ac2d95dffcd2febfae5df098b1577776e2b4`  
		Last Modified: Wed, 30 Nov 2022 22:22:22 GMT  
		Size: 1.7 MB (1703388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a3c36f0f232387119c44145dd35f68a589d293ea19f9fbff2f5dabfba05b7c`  
		Last Modified: Wed, 30 Nov 2022 22:22:21 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92740214b90b0b116f7b164af3e785bb3999df1307a4eac482afb0eedbf3904b`  
		Last Modified: Wed, 30 Nov 2022 22:22:21 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aa99c3b42a7802ab291e3a03628e3b1e204e07e026131426b4752154165dfa`  
		Last Modified: Wed, 30 Nov 2022 22:24:34 GMT  
		Size: 11.8 MB (11822953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9847e4e08f0a216659ffdca72fff5097a0c55c48136c5aa89e2b79f88a1e41b9`  
		Last Modified: Wed, 30 Nov 2022 22:24:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00dc09e12d32f24f556d5d0b90482e6d28d44a02e9a33d1ae612fce07f9d0ea`  
		Last Modified: Wed, 30 Nov 2022 22:25:34 GMT  
		Size: 10.6 MB (10598408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a8b6b5af9a89bb9fbaf0568babe82eb57728a256e471fde0df7db8c192fef7`  
		Last Modified: Wed, 30 Nov 2022 22:25:31 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5132991546f45911c775b89d678af4164e36fc94c0011cc6ab101d6ed4f745a7`  
		Last Modified: Wed, 30 Nov 2022 22:25:32 GMT  
		Size: 18.7 KB (18744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88052201c2226f700e3888bcd7df66fea68357b7b456ca8964b7885efb2e6926`  
		Last Modified: Wed, 30 Nov 2022 22:25:31 GMT  
		Size: 8.6 KB (8622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e618c9a3f671b79927236731a51ae58f4150ad254fe25fcac3fb44999ab04`  
		Last Modified: Thu, 01 Dec 2022 23:02:05 GMT  
		Size: 485.3 KB (485264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c105fd5bae826dbc2e60ee4326bd9355df1e060ecb195cdfab682abd2e16542`  
		Last Modified: Thu, 01 Dec 2022 23:02:05 GMT  
		Size: 3.2 MB (3219697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f198ab170f9ff27991bddfb098158f3ec2cbae8cccbe082ed7632ad560c6e1`  
		Last Modified: Fri, 09 Dec 2022 01:00:15 GMT  
		Size: 1.9 MB (1862817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538cc164df9c0c6478ed222fb0f2a17029997eb59e0fb4caa157624969b43c18`  
		Last Modified: Fri, 09 Dec 2022 01:00:14 GMT  
		Size: 1.6 KB (1599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:5df4d75b4cc6cbf4d28b72eb1dae282a3b480b01688812c92ceb956e74159aa8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35217796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e877bc224ae8ce5aa37acbe91f27f68428e750946a0e3bac33433b353e76ee76`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:03:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:03:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:03:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:03:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:03:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:03:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:03:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:03:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:15:22 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:15:22 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:15:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:15:22 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:15:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:15:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:22:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:22:50 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:22:51 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:22:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:22:51 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:22:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:22:51 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:22:52 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:22:52 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 22:49:44 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 22:49:45 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 22:52:58 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 01:16:05 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:16:05 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:16:05 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:16:05 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:16:06 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 01:16:06 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 01:16:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 01:16:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd5030e0243953a5dc6a26415ada440038b253ef4560edd576a683164696fa9`  
		Last Modified: Wed, 30 Nov 2022 21:30:42 GMT  
		Size: 1.9 MB (1855650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0610361d296c40b235c4e28b9de89b2c1b01a138ea0571a3f566a92befab06`  
		Last Modified: Wed, 30 Nov 2022 21:30:42 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7fe1fcb7369b3185e4af858150e5942b7629718ae79fb697218cb0ab696b3f`  
		Last Modified: Wed, 30 Nov 2022 21:30:42 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e371242642ddc26b7bc5423bdd7e641b9c26a0fc7aed9b6129657090a50e11e`  
		Last Modified: Wed, 30 Nov 2022 21:32:07 GMT  
		Size: 11.8 MB (11822987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec41d52e61fc21b4d57e356a3f45b6690f2bfa90c3fdafabc2e3790aceeccdfc`  
		Last Modified: Wed, 30 Nov 2022 21:32:06 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1bb889a09327675cc91135d1fd9469bd718d65a35fef3798fe98325c6a4f63`  
		Last Modified: Wed, 30 Nov 2022 21:32:49 GMT  
		Size: 12.5 MB (12453784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e9966801143333097c91ac5a40a994f86fce301bdd600836d175d167edacfa`  
		Last Modified: Wed, 30 Nov 2022 21:32:47 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad4c6ddb4a9eafa717d22d7ef16bcd69fbb378e5a3f8d2551bd6c21e7fa726e`  
		Last Modified: Wed, 30 Nov 2022 21:32:47 GMT  
		Size: 18.7 KB (18748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4308fde820d9bff0cbfef3318fdfec18c9c914c198d8151c28860607b8bbf6e`  
		Last Modified: Wed, 30 Nov 2022 21:32:47 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f5e29be8f7ad195f6ab7a9abb7e223ff0981408c747f4241c85c0ceefa9d5`  
		Last Modified: Thu, 01 Dec 2022 22:54:10 GMT  
		Size: 547.5 KB (547509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8867ada66b860358bafba18c70d8019df2c52233366481a4a69bdf208af227f6`  
		Last Modified: Thu, 01 Dec 2022 22:54:10 GMT  
		Size: 3.4 MB (3382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fded8a3b902d1ec2fbb69a34fc435c7bebaf421b0bc2e1a699882bb35057c0ba`  
		Last Modified: Fri, 09 Dec 2022 01:17:06 GMT  
		Size: 1.9 MB (1862867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689dff6df2fd8bb9adceb16a7a1c75d42811012161669625265b8410fb2af340`  
		Last Modified: Fri, 09 Dec 2022 01:17:06 GMT  
		Size: 1.6 KB (1600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:782197fc233d5c8ba28000bccfc9a0aa6808350cbf6d868d159114f3f9f22942
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35750188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:872a207f133af4e8074230a2d68904a22156e585452a2c34bde7f0697eabc6a0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:38:24 GMT
ADD file:f2fbc3153694110f7004f005c4e18435b171ed44a3b35498a1b4916ef1e9af43 in / 
# Tue, 22 Nov 2022 22:38:25 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:07:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:07:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:07:38 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:07:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:07:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:07:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:07:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:07:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:19:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:19:26 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:19:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:19:28 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:19:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:19:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:26:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:26:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:26:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:26:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:26:22 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:26:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:26:24 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:26:25 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:26:26 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 22:40:32 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 22:40:34 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 22:41:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 01:13:51 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:13:52 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:13:53 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:13:54 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:13:56 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 01:13:58 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 01:13:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 01:13:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3cc7ae06783159e8c992cfb745833f904e836c74a7704b7a90b4b45a598f878c`  
		Last Modified: Tue, 22 Nov 2022 22:39:08 GMT  
		Size: 3.4 MB (3408493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1915555ddacfd8951122a364c8e9629d63703005ba29cd220a628087a4564dd6`  
		Last Modified: Wed, 30 Nov 2022 21:37:44 GMT  
		Size: 2.0 MB (1970983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c764cb50f35c195b5559104acb5bb5c203ad771c1de6c4dfe9f876b73d885cb`  
		Last Modified: Wed, 30 Nov 2022 21:37:44 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e72bb2c33f6f2a2dfb7dfe3d1921113cae9107fcf7c76998dc5899bb773ee`  
		Last Modified: Wed, 30 Nov 2022 21:37:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f7e06046353bdba335002b5db04c4a5a30bd60f25e21269860d0677b8bc09d`  
		Last Modified: Wed, 30 Nov 2022 21:39:34 GMT  
		Size: 11.8 MB (11822856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8e4a95e349a05bf3ca0143ba685acfa5f95137d984d8d848d2188cba5b2cbd`  
		Last Modified: Wed, 30 Nov 2022 21:39:33 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d682cb980c4cfa97bd89aaf836592cdafa94dfbd88794db78f8ab10f2447c365`  
		Last Modified: Wed, 30 Nov 2022 21:40:29 GMT  
		Size: 12.7 MB (12748398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dc1cf745cc83e511e4497374be6873c4a45320a122d872286b4bfdefddb9e2`  
		Last Modified: Wed, 30 Nov 2022 21:40:27 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b8d2fb95518fc849cec1182da728685c4003e4cbcc1e5fff7b9d794577f908`  
		Last Modified: Wed, 30 Nov 2022 21:40:27 GMT  
		Size: 18.9 KB (18858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141958d7776a962f07b4123ae18077f451fbd7c2ba931d0fa60272e8d848096`  
		Last Modified: Wed, 30 Nov 2022 21:40:28 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546047446e84762a610b8f3bc6684bcb98bd091a714c6dbac3a115cd494c16ab`  
		Last Modified: Thu, 01 Dec 2022 22:42:48 GMT  
		Size: 542.4 KB (542439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d14be7d35728e0b749e53d7526bb12e9babb49aba14550de7657b023244b4e`  
		Last Modified: Thu, 01 Dec 2022 22:42:49 GMT  
		Size: 3.4 MB (3360832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaec06f3ee0482309beab989e9949feb8d11b47f3a6287d86c1c57bfe18ceec`  
		Last Modified: Fri, 09 Dec 2022 01:15:27 GMT  
		Size: 1.9 MB (1862713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105159fd10670cf578afa5438ae995f1ed007f0e7b1082519a89fd03c99d7d1b`  
		Last Modified: Fri, 09 Dec 2022 01:15:26 GMT  
		Size: 1.6 KB (1599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:fa9a3ef4d5b329e652146e461e6c4e984c3c94a3db78989b0bdd53f7b05ff079
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35710790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ba10e2ef4734ab3b17251f0522926d5e7bcc83d3c9d2d05880ee763c3eea4d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:38:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:38:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:38:42 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:38:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:38:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:38:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:38:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:38:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:51:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:51:58 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:51:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:51:58 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:52:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:52:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:59:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:59:49 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:59:51 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:59:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:59:51 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:59:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:59:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:59:53 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:59:54 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 23:23:58 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 23:24:01 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 23:24:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 01:24:18 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:24:18 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:24:18 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:24:19 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:24:21 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 01:24:22 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 01:24:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 01:24:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0b5b6ebfcb59d7bb376eda2a3a450213bafa678bcca93b0af952b4d0c1c18`  
		Last Modified: Wed, 30 Nov 2022 22:10:33 GMT  
		Size: 1.9 MB (1938378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed945cdf32e78d05dd306e297a89c2b21ac37e2c170d24aa2f5194ea02358fb`  
		Last Modified: Wed, 30 Nov 2022 22:10:32 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bed7d0ee32d4b74590d0ef4b007add6ad78f90481324806ba82f06942037372`  
		Last Modified: Wed, 30 Nov 2022 22:10:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398356f2e403ca0472753695027be1909d3f3cb1411916ce2d8d8bf10d616b8d`  
		Last Modified: Wed, 30 Nov 2022 22:12:22 GMT  
		Size: 11.8 MB (11822989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88071835428ed10c48e3c0942127b9eca7ca19e09e30eef6573bcabb193008a4`  
		Last Modified: Wed, 30 Nov 2022 22:12:20 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532756c0ea4f849c752e37e3cb048f62c42f9d5e13ee842b4b76c55dc7e973a5`  
		Last Modified: Wed, 30 Nov 2022 22:13:23 GMT  
		Size: 12.8 MB (12836330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6c4ec23a6ea75b6bd5687d7e725758f7735edab2e158fa0420ebb00f77dc9a`  
		Last Modified: Wed, 30 Nov 2022 22:13:19 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4474d4487d1bd15c6abd8f1918a088cd4b1d629fdad54d70df1c45790d1e45cf`  
		Last Modified: Wed, 30 Nov 2022 22:13:19 GMT  
		Size: 18.7 KB (18733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a77b03f270f05cb6dd4e0095d0a7a4a258822ee3cdc5a309cf24569cae68a`  
		Last Modified: Wed, 30 Nov 2022 22:13:19 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20021fc58afccbc23cd7652093057ad93e74e1f9512c228a0c65a5d0551730e`  
		Last Modified: Thu, 01 Dec 2022 23:26:49 GMT  
		Size: 565.7 KB (565707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4cc5d90e4823b395d86609e6ca790f9f6efdb05984d23e42a13e1e862f84b6`  
		Last Modified: Thu, 01 Dec 2022 23:26:49 GMT  
		Size: 3.3 MB (3266606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60ff05f47677f5a54684c00849a643c5024aefad5f5d10c160c8e6ec8ae9335`  
		Last Modified: Fri, 09 Dec 2022 01:26:06 GMT  
		Size: 1.9 MB (1862855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abe4bc1f670a53055c9cb0fdd1a60b7f29e1f625ebc984c84f114fef4f94b93`  
		Last Modified: Fri, 09 Dec 2022 01:26:06 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; s390x

```console
$ docker pull postfixadmin@sha256:be3dca528520c6b60b4253b2f3efb6eea2140a69f50fb271e8693cc6edc0ed38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33978916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3153f0e03949ba6bf36f124fd1e7fa902ffa4f37fd4c7a1217290aefae4ad825`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 20:56:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 20:56:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 20:56:11 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 20:56:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 20:56:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:06:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 30 Nov 2022 21:06:24 GMT
ENV PHP_VERSION=8.1.13
# Wed, 30 Nov 2022 21:06:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Wed, 30 Nov 2022 21:06:24 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Wed, 30 Nov 2022 21:06:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 30 Nov 2022 21:06:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:12:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 30 Nov 2022 21:12:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 30 Nov 2022 21:12:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 30 Nov 2022 21:12:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 30 Nov 2022 21:12:26 GMT
WORKDIR /var/www/html
# Wed, 30 Nov 2022 21:12:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 30 Nov 2022 21:12:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 30 Nov 2022 21:12:27 GMT
EXPOSE 9000
# Wed, 30 Nov 2022 21:12:27 GMT
CMD ["php-fpm"]
# Thu, 01 Dec 2022 22:44:18 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 01 Dec 2022 22:44:20 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 01 Dec 2022 22:45:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 09 Dec 2022 01:33:03 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:33:04 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:33:04 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 09 Dec 2022 01:33:05 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 09 Dec 2022 01:33:08 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 09 Dec 2022 01:33:08 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 09 Dec 2022 01:33:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 09 Dec 2022 01:33:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6609bd910046178bd3eac570c2c1fc59cad29fb887adaab5d6693e71d47026`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 1.9 MB (1910084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc11912a116f8a8ce368f5345478751ea66ff55a5b6f480e750cb6e236b8691`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c64f2471f65bf6185d022a4d96096ed5e3f00c2a9697e44113bd0c8728997e1`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed6fc5024408f03633bfa793ab06806085ad1584a6617a0f5f41308e4c749cc`  
		Last Modified: Wed, 30 Nov 2022 21:23:17 GMT  
		Size: 11.8 MB (11823003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ead692d941732ef9bbf199ecc93891c0842e3597a012789484801290c62789e`  
		Last Modified: Wed, 30 Nov 2022 21:23:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be3b8c277ebba63413611c91c47b316e019db0b0ee4260f9f7138f99922ac3`  
		Last Modified: Wed, 30 Nov 2022 21:23:55 GMT  
		Size: 11.6 MB (11607742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61007c491331fadc5a4991ba62bc129dadd06e00160ba8906161b210477c636`  
		Last Modified: Wed, 30 Nov 2022 21:23:53 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfc16ebe43df12c6f8190f7af4725ff72ca695c2af294db2c34105d5a935690`  
		Last Modified: Wed, 30 Nov 2022 21:23:53 GMT  
		Size: 18.8 KB (18761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970045a0914f289bea4656bbee7c44f8ad19a64c13aaaea6f13cc1f647c206a7`  
		Last Modified: Wed, 30 Nov 2022 21:23:53 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f3b5c9749f790bc8f794955a8e5c8d86d219a53cf467807a23915485ee094b`  
		Last Modified: Thu, 01 Dec 2022 22:46:51 GMT  
		Size: 519.7 KB (519671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8327f5a7d301a8994538ec2b921492ea14977bd70bb936b6ca144162f3746e0e`  
		Last Modified: Thu, 01 Dec 2022 22:46:51 GMT  
		Size: 3.1 MB (3051299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b504e567a4d83b8ba804f05c92587e0df23ec79c8b5430c3be53bc3d541e33`  
		Last Modified: Fri, 09 Dec 2022 01:34:34 GMT  
		Size: 1.9 MB (1862851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cca1b5c96d2ac96db2233d515898541e0b00be71dd849a8545cf53423dfcdf3`  
		Last Modified: Fri, 09 Dec 2022 01:34:34 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
