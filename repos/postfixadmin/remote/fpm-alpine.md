## `postfixadmin:fpm-alpine`

```console
$ docker pull postfixadmin@sha256:525bfcf868cdd1e6fad983287ec552a4255491c856fd77fb7a8a683ab26ec65d
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

### `postfixadmin:fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:f91b02a1f8dc537cb65f4c613836d61f7c3934fbeefc841273d0b226f0c27f61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35306166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e59145dfc3b12db5ae1d77c8ad0aa73ecc323385364d30b71c75629c6d40d5b7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:17:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 10:17:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 10:17:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 10:17:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 10:17:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 10:41:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:36:21 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:36:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 01:13:15 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 01:13:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Feb 2023 01:13:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:20:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 01:20:41 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:20:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 01:20:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 01:20:43 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 02:16:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 04 Mar 2023 02:16:07 GMT
STOPSIGNAL SIGQUIT
# Sat, 04 Mar 2023 02:16:07 GMT
EXPOSE 9000
# Sat, 04 Mar 2023 02:16:08 GMT
CMD ["php-fpm"]
# Sat, 04 Mar 2023 04:11:34 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 04 Mar 2023 04:11:35 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 04 Mar 2023 04:12:04 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 04 Mar 2023 04:12:04 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:12:04 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:12:04 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:12:04 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:12:05 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 04 Mar 2023 04:12:05 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Sat, 04 Mar 2023 04:12:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Mar 2023 04:12:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80fdb865a69a85ee910e603ec69d253469dd9367105df81057c89ef565ab971`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.9 MB (1869555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4dbeadc75c19cda75784e259745d42dd938cf860218f8fec2103bf0852be3c7`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257b31b3391b9ce8882eab2c50f2cb64279987f785eeba45218d0b14aa3d74cb`  
		Last Modified: Sat, 11 Feb 2023 11:20:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd1d4b30c9bdbbb2d4259e894f0fc2f28727a5cc972e807de8f2d629b94f3e8`  
		Last Modified: Thu, 16 Feb 2023 01:43:06 GMT  
		Size: 11.8 MB (11781443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3decc859a6af6b2648ca06f8d3b0a889e978ba8d9446cdb20a9c3544e96164`  
		Last Modified: Thu, 16 Feb 2023 01:43:05 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2758a1adb87667936cbd81fe061167d4b185a41882516b4b840cf3397e8844b`  
		Last Modified: Thu, 16 Feb 2023 01:43:31 GMT  
		Size: 12.5 MB (12476368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b79e828bbb7d2457fc3ba0c83ead8daa1b76bdbdd81464b5544033ab08e779`  
		Last Modified: Thu, 16 Feb 2023 01:43:29 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc51b4a824a7d02de1c7517b6df6784d9a554654539621676f48e2bbdc1d22c`  
		Last Modified: Thu, 16 Feb 2023 01:43:29 GMT  
		Size: 18.9 KB (18943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fce5673fba1f8687f9b941017a5b8c874a43b141c96cecb6579d15269bdbff`  
		Last Modified: Sat, 04 Mar 2023 02:31:01 GMT  
		Size: 8.9 KB (8884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9708535f68a713de7c119ca1f52aa28263437e086e25b05816476cca63d748`  
		Last Modified: Sat, 04 Mar 2023 04:12:41 GMT  
		Size: 501.3 KB (501310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b011a869717cddf5e82489d96b2854f23adf9d609ba99d0bf096c4a98d0fef`  
		Last Modified: Sat, 04 Mar 2023 04:12:40 GMT  
		Size: 3.4 MB (3406288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293ecc961cf1a8db4ce8bb15f96b6f2e4e844b9a2e2552b42492e020ce2ee345`  
		Last Modified: Sat, 04 Mar 2023 04:12:40 GMT  
		Size: 1.9 MB (1862856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a344af3aaca3e8e360aff67898ee6e2c11ba0a97666f890d222ee34ed2b892`  
		Last Modified: Sat, 04 Mar 2023 04:12:40 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:d7f28725279cbb990c81fb081998248882ef699edcba96241f7cf2b9a6a41b86
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33516847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022144cf32978d756bff450eee4255cf1bf70ca873400dadae05716553e9e389`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 21:07:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 13 Mar 2023 21:07:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 13 Mar 2023 21:07:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 13 Mar 2023 21:07:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 13 Mar 2023 21:07:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 13 Mar 2023 21:07:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 13 Mar 2023 21:07:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 13 Mar 2023 21:07:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 13 Mar 2023 21:41:15 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 16 Mar 2023 21:58:12 GMT
ENV PHP_VERSION=8.1.17
# Thu, 16 Mar 2023 21:58:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Thu, 16 Mar 2023 21:58:12 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Thu, 16 Mar 2023 21:58:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 21:58:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:03:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 22:03:18 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:03:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 22:03:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 22:03:19 GMT
WORKDIR /var/www/html
# Thu, 16 Mar 2023 22:03:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Mar 2023 22:03:20 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 22:03:20 GMT
EXPOSE 9000
# Thu, 16 Mar 2023 22:03:20 GMT
CMD ["php-fpm"]
# Thu, 16 Mar 2023 23:16:13 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 16 Mar 2023 23:16:15 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 16 Mar 2023 23:16:44 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 16 Mar 2023 23:16:45 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Thu, 16 Mar 2023 23:16:45 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Thu, 16 Mar 2023 23:16:45 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Thu, 16 Mar 2023 23:16:45 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Thu, 16 Mar 2023 23:16:46 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 16 Mar 2023 23:16:46 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:16:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 23:16:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b525ba211658332771b8d1e1e6274a63819ca62cce4ae60af48bd6ea6de2e81e`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.9 MB (1865508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f3139761283dde8c51dccb6f9887eedcebb955cb74f916390ef170c7f432c`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d473bc0ad5e16dc9e7a8b062b4d46e1bc4c325a792b684246fdf4710b85a59`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87250ed138aa623a8b2f33c0a0fd421738734f5fc862fd3d104c3c13f6db76b`  
		Last Modified: Thu, 16 Mar 2023 22:22:31 GMT  
		Size: 11.8 MB (11839131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac970f91bc25e63d502d2c8c1424edd83b28acfb46c890921bf5fe4cc5ac579`  
		Last Modified: Thu, 16 Mar 2023 22:22:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9672413a36f032af7cefde634183027fca8371217ccec7ab8107623f46c8b7`  
		Last Modified: Thu, 16 Mar 2023 22:23:11 GMT  
		Size: 11.3 MB (11282403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3da11e1ece960c965b9fe9cb7f5c2a5f33e16fb9bad118d244dd42e0194dd44`  
		Last Modified: Thu, 16 Mar 2023 22:23:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce02b648c39a2ac2295bdd5aba20a74abe5ea0736b398498e6af1192b0f07b2`  
		Last Modified: Thu, 16 Mar 2023 22:23:08 GMT  
		Size: 18.7 KB (18730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c175dd42632dad2484ac13ec2374c676415e5c0425345362de1882c6285d92`  
		Last Modified: Thu, 16 Mar 2023 22:23:08 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc45533745f832c33087ccb570bbce1c8ac66a2f98233fea5473e8229d4826`  
		Last Modified: Thu, 16 Mar 2023 23:17:07 GMT  
		Size: 527.7 KB (527701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15d9e2a8d6c8ea0281280bccd1319f0a10d3631074a672b52316d7da0d699f`  
		Last Modified: Thu, 16 Mar 2023 23:17:07 GMT  
		Size: 3.0 MB (2994686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be236c586509932f9181403573d93b829f9c43a711103720abf374a1afbae28f`  
		Last Modified: Thu, 16 Mar 2023 23:17:08 GMT  
		Size: 1.9 MB (1862855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303c816372eb196205e1bf95bce186914daed06282dc050f52a4810f72c5d38d`  
		Last Modified: Thu, 16 Mar 2023 23:17:07 GMT  
		Size: 1.6 KB (1595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:b8970e00c5fc42d1bad75a8a72408868bebcafddb6222751a196858a46112adb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32574777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2bf61d01c867e4390c708a97cd7aa4c81635f89b5aafe5afca09e600442c17`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 21:36:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 21:36:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 22:12:31 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Mar 2023 22:12:31 GMT
ENV PHP_VERSION=8.1.16
# Wed, 01 Mar 2023 22:12:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Wed, 01 Mar 2023 22:12:31 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Wed, 01 Mar 2023 22:12:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Mar 2023 22:12:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 22:17:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 22:17:31 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Mar 2023 22:17:32 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 22:17:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 22:17:33 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 02:09:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 04 Mar 2023 02:09:13 GMT
STOPSIGNAL SIGQUIT
# Sat, 04 Mar 2023 02:09:13 GMT
EXPOSE 9000
# Sat, 04 Mar 2023 02:09:13 GMT
CMD ["php-fpm"]
# Sat, 04 Mar 2023 04:24:02 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 04 Mar 2023 04:24:03 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 04 Mar 2023 04:24:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 04 Mar 2023 04:24:30 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:24:30 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:24:30 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:24:30 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:24:31 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 04 Mar 2023 04:24:31 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Sat, 04 Mar 2023 04:24:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Mar 2023 04:24:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9169ee53f4934f506408e6416f765930339b501b32c7cc932909cc1f0c22190`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 1.7 MB (1715927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c652394f365d675be459982d3ff25a0cd449736b35738b11ada9fbcd26323603`  
		Last Modified: Wed, 01 Mar 2023 23:08:08 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8004a620a679d75c3c87ee59d53822c6d18bd9cb75d9bb8e515e1aa829e823e`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313278bb8a497a4e3d6cf40fb986aaef456b1f335ed8a52a9de11b0b6475b77b`  
		Last Modified: Wed, 01 Mar 2023 23:13:54 GMT  
		Size: 11.8 MB (11781418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60dd1bdec9a9b15528ace566530f2a3617906f2c384615aba2bd00cb5297f6`  
		Last Modified: Wed, 01 Mar 2023 23:13:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5423f9e5d77d8080051a256b3b1bb81ecc7a51fcb029c47788116d1469fb82b4`  
		Last Modified: Wed, 01 Mar 2023 23:14:30 GMT  
		Size: 10.6 MB (10600542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6cb3130809d414813a69cc161d21fc4d0465c54113fea94337b71ca74a6e85`  
		Last Modified: Wed, 01 Mar 2023 23:14:25 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d77c0039e2c7efcc7f01e25770d82a5f9aa8121887164875416fb7b1f70a0`  
		Last Modified: Wed, 01 Mar 2023 23:14:25 GMT  
		Size: 18.7 KB (18741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fd5d5d9f1061f0661451194b29efdbc20123e79e58c0fd6f0337ee14ea6c01`  
		Last Modified: Sat, 04 Mar 2023 02:34:05 GMT  
		Size: 8.9 KB (8885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59146321ca6ec51867ada369e1daf145947ad5db48bd3571ff567c797536e638`  
		Last Modified: Sat, 04 Mar 2023 04:25:38 GMT  
		Size: 485.4 KB (485397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37ab70adc1f746c89e1e79bc6acc6a7e90958db615f494584b9322fa656cf06`  
		Last Modified: Sat, 04 Mar 2023 04:25:38 GMT  
		Size: 3.2 MB (3226447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2731bebdc1a3aaae19ae10cd6d809139f5ed13aebec2f13d63b2fcc5d3357157`  
		Last Modified: Sat, 04 Mar 2023 04:25:38 GMT  
		Size: 1.9 MB (1862856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02201d87e424e480e560675043fd8dafa2b2d99996e43c751d7db2794d248801`  
		Last Modified: Sat, 04 Mar 2023 04:25:37 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:32dabc5a2e452a4281485fb4a59958364fca9420eb8479f3a86443d8443a0785
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35528561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45bfe169957f1dc3eca4f887a30cb90402c6b36aac397a4a2dba77923ca520c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:02:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:02:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:02:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:02:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 02:02:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 02:02:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:02:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:02:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 02:26:41 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 16 Mar 2023 22:46:24 GMT
ENV PHP_VERSION=8.1.17
# Thu, 16 Mar 2023 22:46:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.17.tar.xz.asc
# Thu, 16 Mar 2023 22:46:24 GMT
ENV PHP_SHA256=b5c48f95b8e1d8624dd05fc2eab7be13277f9a203ccba97bdca5a1a0fb4a1460
# Thu, 16 Mar 2023 22:46:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 22:46:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:53:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 22:53:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:53:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 22:53:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 22:53:53 GMT
WORKDIR /var/www/html
# Thu, 16 Mar 2023 22:53:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Mar 2023 22:53:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 22:53:53 GMT
EXPOSE 9000
# Thu, 16 Mar 2023 22:53:53 GMT
CMD ["php-fpm"]
# Fri, 17 Mar 2023 00:21:29 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 17 Mar 2023 00:21:30 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 17 Mar 2023 00:21:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 17 Mar 2023 00:21:54 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Fri, 17 Mar 2023 00:21:54 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 17 Mar 2023 00:21:54 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Fri, 17 Mar 2023 00:21:54 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Fri, 17 Mar 2023 00:21:55 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 17 Mar 2023 00:21:55 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Fri, 17 Mar 2023 00:21:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 17 Mar 2023 00:21:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65da1d1bbae15a06f79c4d79d885439cb51d02c27c69741770a1ace04a962454`  
		Last Modified: Sat, 11 Feb 2023 03:02:23 GMT  
		Size: 1.9 MB (1862646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53689469854ea07050d653c2567c0a362a36bf42c1db6ad7ca78f0ce04d4a862`  
		Last Modified: Sat, 11 Feb 2023 03:02:22 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c363c99e0af7af0ce7cc0c3b401461324b37d279159235d225fb19c056c4c1`  
		Last Modified: Sat, 11 Feb 2023 03:02:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae469d56f20af5a61130c4d6c901b88b3ec2aa3fab5426162759c5754f967369`  
		Last Modified: Thu, 16 Mar 2023 23:22:55 GMT  
		Size: 11.8 MB (11839138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69b34370b9b6ac4f8e6577a4d29727f73c42d6d1b059efd35246ef2ee89ec02`  
		Last Modified: Thu, 16 Mar 2023 23:22:54 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e21412f8ff9230ddacce5c1d5a2bf7b9fcd2654acecdaa3ea8c3fe3ba4001eb`  
		Last Modified: Thu, 16 Mar 2023 23:23:24 GMT  
		Size: 12.7 MB (12734622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d013094faeed712ac5f23406f6c3cd7856fad87106e10324a7d8d0be1c52523d`  
		Last Modified: Thu, 16 Mar 2023 23:23:22 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53bbdc441ab22fee096df2145c84b53143925642b0360f0d04fd4a9f86c5351`  
		Last Modified: Thu, 16 Mar 2023 23:23:23 GMT  
		Size: 18.8 KB (18787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a28ef0323fc76ef468d42edf158f65c48fbf627dbba2b9ce501ce0beb8f429`  
		Last Modified: Thu, 16 Mar 2023 23:23:23 GMT  
		Size: 8.9 KB (8875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dc839d97e964e89d232f53b2ca79195a83405587cef0eb03af5437ab992679`  
		Last Modified: Fri, 17 Mar 2023 00:23:08 GMT  
		Size: 547.7 KB (547659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486d342d5e5f04c04697de17499b00d388bc575c94e5c75c65774ba7ae74553f`  
		Last Modified: Fri, 17 Mar 2023 00:23:09 GMT  
		Size: 3.4 MB (3385959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19169fd7f0da5e8f66aeeb7b0d32e705a8e87e4928ae501c2769d822c25f0ef`  
		Last Modified: Fri, 17 Mar 2023 00:23:09 GMT  
		Size: 1.9 MB (1862846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5eb5bb381ad223437148cf7d51a03391785d3260889de680e5964f778d0258`  
		Last Modified: Fri, 17 Mar 2023 00:23:08 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:c5e4cd0541fff2b9993b9268824116433faa92c50159bdbb619e835e57099514
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35742890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b58aa0452f8873be719603e96214797a437f0d2b007cf2c2ca8d4448ce06783`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 15:08:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 15:08:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 16:30:36 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Mar 2023 16:30:36 GMT
ENV PHP_VERSION=8.1.16
# Wed, 01 Mar 2023 16:30:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Wed, 01 Mar 2023 16:30:36 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Wed, 01 Mar 2023 16:30:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Mar 2023 16:30:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 16:42:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 16:42:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Mar 2023 16:42:39 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 16:42:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 16:42:39 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 02:46:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 04 Mar 2023 02:46:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 04 Mar 2023 02:46:04 GMT
EXPOSE 9000
# Sat, 04 Mar 2023 02:46:04 GMT
CMD ["php-fpm"]
# Sat, 04 Mar 2023 04:46:02 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 04 Mar 2023 04:46:03 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 04 Mar 2023 04:46:33 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 04 Mar 2023 04:46:33 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:46:33 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:46:33 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 04:46:33 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 04:46:35 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 04 Mar 2023 04:46:35 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Sat, 04 Mar 2023 04:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Mar 2023 04:46:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5394292b2b83b2b876e0f3301349b0299305f8034ed3fa062d20c20268efbd52`  
		Last Modified: Wed, 01 Mar 2023 18:23:52 GMT  
		Size: 2.0 MB (1991827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e923c580cf6f27c534dc0869dfae4f7e9e424c149940e20be2ffef7aa344c424`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c6096004f76a359d1c0d104682a61452036bae13908723157c118939b617b6`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323bafca8b70cf53c03b05a398a86b1be57949a568cc33b70df05d3834427111`  
		Last Modified: Wed, 01 Mar 2023 18:29:50 GMT  
		Size: 11.8 MB (11781434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b297fe0b878d5b4a076cf7df76691b4042ddaad29830043f034f721d724a18a`  
		Last Modified: Wed, 01 Mar 2023 18:29:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3e4018e8dab7682bd9509b1a44c6bb1156a3f83caec27acdabf3d7ed23990e`  
		Last Modified: Wed, 01 Mar 2023 18:30:27 GMT  
		Size: 12.8 MB (12754994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d64d63d5779a4452a5400c2501b1df3ab24f2bfe7c3afc6c168cc26229a451f`  
		Last Modified: Wed, 01 Mar 2023 18:30:23 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bde6cb72b9c058053dd4135377b88befffba3bd3a0b51443749a0afb6b103b`  
		Last Modified: Wed, 01 Mar 2023 18:30:23 GMT  
		Size: 18.9 KB (18925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb36e71e10ed56f5203ad3f42085904a40a357f8c75c37060a0926dfc5bd369`  
		Last Modified: Sat, 04 Mar 2023 03:10:21 GMT  
		Size: 8.9 KB (8885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b970d26723e16208cbea30f71b32cb8bfcf5ca13a295d354b744d60eb03a6a72`  
		Last Modified: Sat, 04 Mar 2023 04:47:42 GMT  
		Size: 542.7 KB (542678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b35ecc7d907843627126638a1341d1f869e1582d13f9d62fd1f1aa31f716ef`  
		Last Modified: Sat, 04 Mar 2023 04:47:42 GMT  
		Size: 3.4 MB (3362870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c77f041cd08dca5a688c7e79cc7bb6fe8c51945a333edb0cd423a3505b141a`  
		Last Modified: Sat, 04 Mar 2023 04:47:46 GMT  
		Size: 1.9 MB (1862857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bf04fa6256c63b9d003a1eaa718f20a376f597aca61fe9264a51e589ecf271`  
		Last Modified: Sat, 04 Mar 2023 04:47:42 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:2d573c96caf6643d50908ef57a153494c5fb6f5981f6f79febe8c982e8ee7af1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35694533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c142637ea85141aff0e576c7af0a0d47a80c2d358e5bb424113a4492448ea1b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:08:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:08:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:08:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:08:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:08:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 10 Feb 2023 23:38:04 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:22:25 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:22:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 01:03:08 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 01:03:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Feb 2023 01:03:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:13:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 01:13:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:13:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 01:13:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 01:13:19 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 02:04:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 04 Mar 2023 02:04:34 GMT
STOPSIGNAL SIGQUIT
# Sat, 04 Mar 2023 02:04:34 GMT
EXPOSE 9000
# Sat, 04 Mar 2023 02:04:34 GMT
CMD ["php-fpm"]
# Sat, 04 Mar 2023 06:17:14 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 04 Mar 2023 06:17:18 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 04 Mar 2023 06:18:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 04 Mar 2023 06:18:18 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 06:18:18 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 06:18:19 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 06:18:19 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 06:18:21 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 04 Mar 2023 06:18:22 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Sat, 04 Mar 2023 06:18:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Mar 2023 06:18:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfa1898e4103c3c306fd301195ab70581ac39be1be2ad84260c45520aaa5d05`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.9 MB (1946683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fded8faaf0ac23f23c9b92d38d3e833d89b91908a65685dd807fc5ed5718e57`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8afe3cb27338f4dc17809e93d8c3ba65ea9bbe27288f937f4e25fb03bc6010`  
		Last Modified: Sat, 11 Feb 2023 00:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03dadd5381bdb2a3bacfe8cf2adc8e43a29b7577e31e5dc948f137404dc28bd`  
		Last Modified: Thu, 16 Feb 2023 01:44:07 GMT  
		Size: 11.8 MB (11781428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76549ae119caf4e1d6999ad0c45fac3faa1c90a7a4f9418a928d857ffcd5e0dc`  
		Last Modified: Thu, 16 Feb 2023 01:44:05 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaabc3ae2f07d5afaa9247b8ffb68c4b2d2c5d720bf08b5f290757eb788e627`  
		Last Modified: Thu, 16 Feb 2023 01:44:45 GMT  
		Size: 12.8 MB (12841985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed36be7cd8470bb136f902b960d20e0dec207ae24beedf1c78a216d1e2ed2fc`  
		Last Modified: Thu, 16 Feb 2023 01:44:41 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4b34965486bb34a097ad0fd9ed8eb4c6dfa66280cabb2945da3232ee0bc12`  
		Last Modified: Thu, 16 Feb 2023 01:44:41 GMT  
		Size: 18.7 KB (18741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79c354c6c8f5e85142d0d7475a7a92bedbe8ee1b316992a9cce51febf3ba953`  
		Last Modified: Sat, 04 Mar 2023 02:23:37 GMT  
		Size: 8.9 KB (8883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcadbd37018725bbe250b154e80156832506552057fd4154fa450625510320`  
		Last Modified: Sat, 04 Mar 2023 06:19:34 GMT  
		Size: 565.9 KB (565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c947e15b53654bad8362da2182f38e50e894d285e460e8528b94a557f1da94e1`  
		Last Modified: Sat, 04 Mar 2023 06:19:34 GMT  
		Size: 3.3 MB (3271286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb796b72fb44fa83cd0a76681b276fdd1c1f222f5be83919d2c47e832a78fa7f`  
		Last Modified: Sat, 04 Mar 2023 06:19:34 GMT  
		Size: 1.9 MB (1862856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f7651d445cae03f53f631a973e41b606952fe369551467d734ba3da7766e31`  
		Last Modified: Sat, 04 Mar 2023 06:19:33 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; s390x

```console
$ docker pull postfixadmin@sha256:857f214e7ed1121f5e7d93fe5e4693e263009d57d7e1043a8787a89de6fe4b8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33956126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e3e4e3d9ddec2013478ee33f91c619374e59d422f20c80129f47b01e1a96b80`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:40:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 03:40:21 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 03:40:22 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 03:40:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 03:40:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 04:00:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:34:21 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:34:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 01:09:02 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 01:09:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Feb 2023 01:09:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:16:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 01:16:26 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:16:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 01:16:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 01:16:27 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 01:02:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 04 Mar 2023 01:02:47 GMT
STOPSIGNAL SIGQUIT
# Sat, 04 Mar 2023 01:02:48 GMT
EXPOSE 9000
# Sat, 04 Mar 2023 01:02:48 GMT
CMD ["php-fpm"]
# Sat, 04 Mar 2023 02:30:57 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 04 Mar 2023 02:30:58 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 04 Mar 2023 02:31:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 04 Mar 2023 02:31:23 GMT
ARG POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 02:31:23 GMT
ARG POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 02:31:23 GMT
ENV POSTFIXADMIN_VERSION=3.3.13
# Sat, 04 Mar 2023 02:31:23 GMT
ENV POSTFIXADMIN_SHA512=bf7daaa089ee3adc4b557f1a7d0509d78979ef688fb725bab795f5c9d81e8774296245fde0cb184db51e9185cad381682c3ecc0bfadf852388b499a0a95cca64
# Sat, 04 Mar 2023 02:31:25 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 04 Mar 2023 02:31:25 GMT
COPY file:3f9cd88c9194b4dd46840502e61fb0ec7c3aa999b086fec7959e90f51a6c13ee in /usr/local/bin/ 
# Sat, 04 Mar 2023 02:31:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Mar 2023 02:31:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e08f96f9a305daacf9ee42f9847666c785231f5db9684aae1648426463f923`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.9 MB (1917113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b2b7eda29298bc923307ecd06eca2607d89341d31329cad08c2ddd6d3dda03`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dc1497b9a6351ab931f19c686d45bea176daa8f6da7db62dce416a091a4944`  
		Last Modified: Sat, 11 Feb 2023 04:35:14 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4aee298950401b047cc7fe683911318270f385ca54d4a123658d52e5603f8e`  
		Last Modified: Thu, 16 Feb 2023 01:38:04 GMT  
		Size: 11.8 MB (11781441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0ce98bebabf870841318129a2c67599d9d5b00779371ccabf96605be56915f`  
		Last Modified: Thu, 16 Feb 2023 01:38:03 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98757c9d68865cd8cb75456f07345862ab3c7efe50d91772b3b84073d8b1a112`  
		Last Modified: Thu, 16 Feb 2023 01:38:28 GMT  
		Size: 11.6 MB (11611279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8288c9ce60e15a40ea5713e3947d0abd2def107c63f4424ceab577350af0d8`  
		Last Modified: Thu, 16 Feb 2023 01:38:27 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d8dc76b7a195228e4dc9aab2b0f9542e93c5162c69d1062391d9bf5589aaa2`  
		Last Modified: Thu, 16 Feb 2023 01:38:27 GMT  
		Size: 18.7 KB (18748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901ece7138bf920e4ec89aa12a0b3b5333f873fe88ff704e2420f07b7ac05c16`  
		Last Modified: Sat, 04 Mar 2023 01:17:48 GMT  
		Size: 8.9 KB (8884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0457d25c02414c7eb7e8ab6b98619ee7e067ebb8975508b97736a6ea10b5f2e`  
		Last Modified: Sat, 04 Mar 2023 02:32:19 GMT  
		Size: 519.7 KB (519720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e046db6e3d1989c7f3df0ecaf536c0d6ac9e6600644a4b2d8d918f824d777610`  
		Last Modified: Sat, 04 Mar 2023 02:32:18 GMT  
		Size: 3.1 MB (3054895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dd1e98f31bb580e2b9248c1fe83cdc440bf647b7c00344406f1f162431796b`  
		Last Modified: Sat, 04 Mar 2023 02:32:19 GMT  
		Size: 1.9 MB (1862855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f28b329560c09362d93f1e3017ffae1a37698932fcf8f00c0fe6005ab4b0f9`  
		Last Modified: Sat, 04 Mar 2023 02:32:18 GMT  
		Size: 1.6 KB (1599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
