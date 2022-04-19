## `joomla:4-php7.4-fpm-alpine`

```console
$ docker pull joomla@sha256:94c7d08c23e94a55be9e6ecb4fa448fcaf8e3ee21b9f896b1531cd46419d14c5
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

### `joomla:4-php7.4-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:af4b9896273b00271ab6703c1147402807967d150678d3569c0488eec86b38a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70061074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f47ca8f3fa6cb2289cb26d6d9ccdf147f8398df1757e495b1e202c67706c3087`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:59:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:59:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:59:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:59:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:59:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:59:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:59:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 02:11:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:03:14 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:03:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:03:14 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:03:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Apr 2022 01:03:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:10:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:10:10 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:10:11 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:10:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:10:11 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:10:12 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Apr 2022 01:10:12 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Apr 2022 01:10:12 GMT
EXPOSE 9000
# Tue, 19 Apr 2022 01:10:12 GMT
CMD ["php-fpm"]
# Tue, 19 Apr 2022 03:41:50 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 19 Apr 2022 03:41:50 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 19 Apr 2022 03:41:51 GMT
RUN apk add --no-cache 	bash
# Tue, 19 Apr 2022 03:43:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 19 Apr 2022 03:43:30 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 03:43:30 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 19 Apr 2022 03:43:30 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 19 Apr 2022 03:43:37 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 19 Apr 2022 03:43:37 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 19 Apr 2022 03:43:37 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 19 Apr 2022 03:43:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 03:43:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f85627e3d0df735c885c9502afee6c4a98aec08c02a0b31ffd6ee36d1d3ed`  
		Last Modified: Tue, 05 Apr 2022 02:49:01 GMT  
		Size: 1.7 MB (1701412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89395091f2959844751d9669bf4ffa0d72cae1e7710bd34d692c4a724abcfe20`  
		Last Modified: Tue, 05 Apr 2022 02:49:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342a00f1dee7a210bf0e6327fce29393f5b0b67b1dbd297a5d39b322c2c61df`  
		Last Modified: Tue, 05 Apr 2022 02:49:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48d140dbee063649d400c1f428b711af96d7c0593db9ec79000611391534af3`  
		Last Modified: Tue, 19 Apr 2022 02:01:47 GMT  
		Size: 10.4 MB (10438866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f615370bed2533fa409a26367161ef5501524d674bad69505dc633e223d6f3`  
		Last Modified: Tue, 19 Apr 2022 02:01:46 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912de62f7806a199c0fd5b2a82dcb093fcb253913fad38298738d1e0b4a3fd6`  
		Last Modified: Tue, 19 Apr 2022 02:02:27 GMT  
		Size: 11.5 MB (11514192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d69dd58167252e5b98470ede276a3273adcf0f1ac1759bd4611b25e6be16a2`  
		Last Modified: Tue, 19 Apr 2022 02:02:25 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6883a9a3107d0e0d2f6a828f240517c9401e7465ed500e1d7b0ee0c468d942`  
		Last Modified: Tue, 19 Apr 2022 02:02:26 GMT  
		Size: 18.4 KB (18444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856907323251c35cff87ca863ebff6cf94b26f0521aec2a1110bc8eb10ccc9fe`  
		Last Modified: Tue, 19 Apr 2022 02:02:25 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7f3823f47cdba9acc0bbfcf65e5c4fb2747fb0fd894406d66371c7683d7e66`  
		Last Modified: Tue, 19 Apr 2022 04:03:06 GMT  
		Size: 467.0 KB (466961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6c8e15f8752636861b2d24814b283575e14618df1b3d3cec9fe3ddb20f45e7`  
		Last Modified: Tue, 19 Apr 2022 04:03:08 GMT  
		Size: 20.7 MB (20747077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4380330b500fce93d3aff42ffc72f4092acf7ff867a97d3a97624b6aec8cea60`  
		Last Modified: Tue, 19 Apr 2022 04:03:09 GMT  
		Size: 22.3 MB (22344213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808279832d4820bbf0aa2e4fa0f2cdb6f5f95e2060b88f95fb712ef893a7d9cb`  
		Last Modified: Tue, 19 Apr 2022 04:03:06 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bab0d9f8747534c12557cd21d2fbcb9e063f704ce92846e8e9d9ab84d2e73a7`  
		Last Modified: Tue, 19 Apr 2022 04:03:05 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:652f7437a110f132f2d59dfc7dc5c1ed1097d98593cde0e0f909bbd9257d6c1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68213065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6830d6ba57c18a97bfdc0fb07f3b771d133c17f39f286dc4f1dbc33f251999`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 04 Apr 2022 23:53:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 04 Apr 2022 23:53:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 04 Apr 2022 23:53:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 04 Apr 2022 23:53:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 04 Apr 2022 23:53:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:55:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 00:55:21 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 00:55:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 00:55:22 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 00:55:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:55:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:05:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:05:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:05:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:05:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:05:26 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:05:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:05:28 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:05:28 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:05:28 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 16:05:27 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 16:05:27 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 16:05:30 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 16:09:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 16:09:57 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 16:09:57 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 16:09:58 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 16:10:17 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 16:10:18 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 16:10:19 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 16:10:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 16:10:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f4857007e05a14c6f648dc95eb29cd4faae7806674bb49c86a9c22bf5c828e`  
		Last Modified: Tue, 05 Apr 2022 01:33:30 GMT  
		Size: 1.7 MB (1688742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0f12cd34ba09b6e733247467586fb1354d26dfc93308155099ca243578518`  
		Last Modified: Tue, 05 Apr 2022 01:33:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc724c09cd88ae23080a3eb4cc057c4cbe9cbd5c83048ea54c647cbcc8f040`  
		Last Modified: Tue, 05 Apr 2022 01:33:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c97bcc795104c2de98712535c04ef105d204ecc5928136f935f1779267adab`  
		Last Modified: Tue, 05 Apr 2022 01:40:46 GMT  
		Size: 10.4 MB (10438279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439911d36b1c5c4c6b268d38a81c986cc80221ea2d276cd24c3540473e010541`  
		Last Modified: Tue, 05 Apr 2022 01:40:44 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725271bdb9923d5064c1077f50747fa38347e7cfb0fd3123991399f8a240bef0`  
		Last Modified: Tue, 05 Apr 2022 01:41:54 GMT  
		Size: 10.7 MB (10705695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7bb07498db082665c6a3c75003b5683f1bc578e81633648e4054e41db9ceae`  
		Last Modified: Tue, 05 Apr 2022 01:41:46 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24eb878017deb9f1f7fed329d19c2e4bde3cc9504073f72f07afb1f2c44ca97`  
		Last Modified: Tue, 05 Apr 2022 01:41:46 GMT  
		Size: 18.4 KB (18388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d0475b1ceccdcc2148eb0d3ab116d655cf55086ad5e8bc9984a5d7b79db5b2`  
		Last Modified: Tue, 05 Apr 2022 01:41:46 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70056de84d8dd3edfc1cc2a565727bc42e121117a5b02f02049ff81ff3969eb1`  
		Last Modified: Tue, 05 Apr 2022 16:27:17 GMT  
		Size: 455.1 KB (455084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3a3bfa46a84fd31e6d307fb26281deb619b4720f654f64525bcfc8a3c73581`  
		Last Modified: Tue, 05 Apr 2022 16:27:25 GMT  
		Size: 19.9 MB (19925329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4cd61d795abcc42c0f1a4ae948c61900c9cf33a7b75e6b0faefeff3e468673`  
		Last Modified: Tue, 05 Apr 2022 16:27:29 GMT  
		Size: 22.3 MB (22344218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f487b8aca07f8c186fe9cdc41e2131f6c60004922f3d75e0b3423647b147d2`  
		Last Modified: Tue, 05 Apr 2022 16:27:17 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbd1dce1fe0b6828898612e7b0db406bfe6e38b360e5ee317875d3c7a332460`  
		Last Modified: Tue, 05 Apr 2022 16:27:17 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:06e5761f8d54c6c9d617ed020c76666e018f3293620d3c0b7e0eadf117249951
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67073612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6002c52e349645ce9fdf37fb093381b85fdbae84b71dc37dc1eb753db1e2ecb1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:44:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:44:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:44:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:44:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:44:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:44:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:44:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:44:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 01:48:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 01:48:33 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 01:48:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 01:48:34 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 01:48:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:48:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:57:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:57:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:57:45 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:57:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:57:46 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:57:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:57:48 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:57:48 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:57:48 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 22:54:10 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 22:54:11 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 22:54:13 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 22:58:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 22:58:29 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 22:58:29 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 22:58:30 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 22:58:48 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 22:58:49 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 22:58:50 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 22:58:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 22:58:50 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e79621416caf77f775491eca7e32b6744cb98a7f314d25662db9d47388f78c`  
		Last Modified: Tue, 05 Apr 2022 02:39:26 GMT  
		Size: 1.6 MB (1556468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e6096135db80ad99d3893e56fed755390988cde114bfa2eadb0344135aa68`  
		Last Modified: Tue, 05 Apr 2022 02:39:26 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e579551e9fe0160cdaf60f2b80ab01b627b8bfea2c89907509913896a5f1b118`  
		Last Modified: Tue, 05 Apr 2022 02:39:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf5539e90d9f05a1b4a2f2e4b1273728a29214113f0ed8b2ba534a584bf98d`  
		Last Modified: Tue, 05 Apr 2022 02:50:11 GMT  
		Size: 10.4 MB (10438275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a1199a632170c64226f7b3d7a421ee9a801bb71e78f3ec48c51d4949add586`  
		Last Modified: Tue, 05 Apr 2022 02:50:08 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646c147963befdac750f05313e281fdb6c2aa12714aaa00538217d20c3cd4cfc`  
		Last Modified: Tue, 05 Apr 2022 02:51:24 GMT  
		Size: 10.1 MB (10065555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a17e2a4ee9ef34cb36805b8a6db450737ed36ffcb28f3e30be7465019e1b3c0`  
		Last Modified: Tue, 05 Apr 2022 02:51:17 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f78b4eeb80b70bcebb9d3f479395dd38dbe1f820a5ace569ddeb8faf9c4a345`  
		Last Modified: Tue, 05 Apr 2022 02:51:17 GMT  
		Size: 18.4 KB (18360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b1a662b90059d60049f0a5fe34f8d9232b5603ac44667d1fbf912d3ca4ff6e`  
		Last Modified: Tue, 05 Apr 2022 02:51:17 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c484bd11afc1a861c99d890d8ba9283ec0eed23643f8b2eb4be90d90e72689`  
		Last Modified: Tue, 05 Apr 2022 23:19:47 GMT  
		Size: 415.5 KB (415518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f9113cd0e7021b04902f92dae46d4ecebec87701cd790a8ee7b478a07e025a`  
		Last Modified: Tue, 05 Apr 2022 23:19:56 GMT  
		Size: 19.8 MB (19795585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d78f96cb17c30feb6bbbc4cd028cde42ac3737d87a5b74145b24115042b39`  
		Last Modified: Tue, 05 Apr 2022 23:20:06 GMT  
		Size: 22.3 MB (22344170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf2dc64c59987e9f2eac1796cd430b8b83c46a0013f83b461d3ef85c2600f01`  
		Last Modified: Tue, 05 Apr 2022 23:19:46 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a619c14313a92593da0b040218e0c9df427900210d585e89e6f5406f2dd067`  
		Last Modified: Tue, 05 Apr 2022 23:19:46 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:4bb4a7632b8053860f9e2bbe7adff85ea58cb52a812dedff565343e4df5e5e3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69639792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb6b3a36971b731a3d470670a78c199c92ba56406f203a10adb098fbe23fa87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:14:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:14:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:14:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:14:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:14:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:14:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:14:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 01:19:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 01:19:21 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 01:19:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 01:19:23 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 01:19:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:19:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:26:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:26:34 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:26:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:26:35 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:26:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:26:37 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:26:38 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:26:39 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 15:11:53 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 15:11:54 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 15:11:56 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 15:13:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 15:13:48 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 15:13:49 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 15:13:50 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 15:13:58 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 15:13:59 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 15:14:00 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 15:14:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 15:14:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69c83c314e8e18362c8a6739f6f7857ed89cc606ea05f0a95d6eb922fbc3f5`  
		Last Modified: Tue, 05 Apr 2022 01:52:13 GMT  
		Size: 1.7 MB (1696240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8f271730dc83953a1ddf4c1d17b33fcb696501a3331a55c9ed5ccfec44542c`  
		Last Modified: Tue, 05 Apr 2022 01:52:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d1df3f0f228d28d8f270e64056adb7297fcca517c48468be36d482e2f383dd`  
		Last Modified: Tue, 05 Apr 2022 01:52:12 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f16d86c481371a872e65142b9a334cba4e8f837b6ad8edeb8adadf9768bacd`  
		Last Modified: Tue, 05 Apr 2022 01:59:01 GMT  
		Size: 10.4 MB (10438056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475496376391d28e2fc16dfc01ba2b7fb1197892c38a490cbd73bf35f06570b1`  
		Last Modified: Tue, 05 Apr 2022 01:59:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0ef4b13b0b5cf6a3838b5c179338140d2ef0bc13760a36007e5c47ebfc9e93`  
		Last Modified: Tue, 05 Apr 2022 01:59:48 GMT  
		Size: 11.3 MB (11264247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4355dbe28edf90cf05624610454ce4fc816ad03e02e62fed2a09a29b1767bb`  
		Last Modified: Tue, 05 Apr 2022 01:59:46 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ea15755d6da512b4a62b12974b374bcdd0fb6e1b25086daa8219945672cff6`  
		Last Modified: Tue, 05 Apr 2022 01:59:46 GMT  
		Size: 18.3 KB (18307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9988dfa1167faac1044a04d658fb38aab74c13958011e77e5d497f8e64057b20`  
		Last Modified: Tue, 05 Apr 2022 01:59:46 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63184f7da5f6d7ffecc8c14b3b558d2fcc35f69427c4f4f2f0cc3ede89d4b198`  
		Last Modified: Tue, 05 Apr 2022 15:23:40 GMT  
		Size: 474.0 KB (473962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5815d79edb920e3f5d00d8c54bb5ab125e219de0c6378fbf2fab34521cffd8`  
		Last Modified: Tue, 05 Apr 2022 15:23:42 GMT  
		Size: 20.7 MB (20671482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb0a6a8232a0abc39b806b732cf51b7d2d335d1e1cdd723cda169279f588149`  
		Last Modified: Tue, 05 Apr 2022 15:23:43 GMT  
		Size: 22.3 MB (22345738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d467215081f764c1e36b029204a92ca957447a3d3eaddac5817bae695a1c291`  
		Last Modified: Tue, 05 Apr 2022 15:23:39 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fbfa15533ee078e1fc9cf97b09cc30665a054732028838c12dfce5c062e39e`  
		Last Modified: Tue, 05 Apr 2022 15:23:39 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:34fb70fde6e3f2154098961b4ed7a5d31e8d08e1d04f88cdff6fe515c40a4e5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70617364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfa764eed5fb865cfe7526f24c08067ee930f3526203f18f585b06f1a3c8bd5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:05:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:05:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:05:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:05:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:05:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:05:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:05:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:05:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:52:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 00:53:00 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 00:53:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 00:53:02 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 00:53:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:53:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:59:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:59:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:59:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:59:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:59:29 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:59:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:59:31 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:59:32 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:59:33 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 08:19:55 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 08:19:56 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 08:19:57 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 08:21:33 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 08:21:34 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 08:21:35 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 08:21:36 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 08:21:45 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 08:21:46 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 08:21:47 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 08:21:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 08:21:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45a8803aeb5badfcbafc3a64d45ef0d99401331488cc5495a9bf7e66c3c475`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 1.8 MB (1800021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8efaa6aa5ded5cf73ecb3fc3a3fb655e5cadfea53b9ab939d90bf4ddb8653d0`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f0f938930408ae4fa469fe3ce2586fc2b3be3450492deeabddfac3f9533860`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa270fcc4681dd20411638ed8bd53ecc3843fdbc335985ec88ba02e05278aa8f`  
		Last Modified: Tue, 05 Apr 2022 01:31:23 GMT  
		Size: 10.4 MB (10438030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cb32c9ab93a48ccb7b5940ea81e8975f19349e49668fe9c6019f5537bc5c5e`  
		Last Modified: Tue, 05 Apr 2022 01:31:21 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37c7036dd6e7ded60021f2312a603b406626b00b74fafc388ac6ab7821172d9`  
		Last Modified: Tue, 05 Apr 2022 01:32:12 GMT  
		Size: 11.7 MB (11729173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1f82b633ac0d76f62d5a0cec229e8ed8654d8c7cae73d605fbca3ea04ce0a8`  
		Last Modified: Tue, 05 Apr 2022 01:32:11 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0838566a7dab73cc1b1b34ce322eb3f25c6082837c767c4e8fca5f8e8e3a6a6`  
		Last Modified: Tue, 05 Apr 2022 01:32:10 GMT  
		Size: 18.3 KB (18287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1f6a2b580a6156fa3ebb9304015ec0f78300aed02841480ad60b047c992702`  
		Last Modified: Tue, 05 Apr 2022 01:32:10 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1a35f5be384bf97783ec3b3a3474e6803884f7a42e8fda079eb6498c5c3502`  
		Last Modified: Tue, 05 Apr 2022 08:31:02 GMT  
		Size: 503.4 KB (503368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910d44f0d2c85d5966f81cad952da806c7bc1a1426ef1ba02c5a8b0a5c337f73`  
		Last Modified: Tue, 05 Apr 2022 08:31:05 GMT  
		Size: 20.9 MB (20948509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9748ebb482ecd22cb65ef4d8d52a485bfce92aafcd2012fb6712df850b855c8`  
		Last Modified: Tue, 05 Apr 2022 08:31:06 GMT  
		Size: 22.3 MB (22345721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cca912e4cbd3b29a1d87e9be01176d4677c7051f48f72f1921a7874bda4f51d`  
		Last Modified: Tue, 05 Apr 2022 08:31:02 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75df7d4ac5c38f0cb9ab09e40c9ad647364aef8c487224080a9a3dfc7b32d2f4`  
		Last Modified: Tue, 05 Apr 2022 08:31:02 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:a3877a682dac6f660d0bc0ed3cdd5d384796fe588cb5fab39812379791bb177d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71102201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b77e6f3607118a46924c6b043fdf3c15add66a5eba1f0020c14237be0376a3c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:16:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 01:16:42 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 01:16:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 01:16:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 01:17:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 01:17:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:17:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:17:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 02:36:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 02:36:16 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 02:36:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 02:36:21 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 02:36:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 02:36:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:47:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 02:47:05 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:47:14 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 02:47:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 02:47:21 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 02:47:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 02:47:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 02:47:36 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 02:47:40 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 21:01:18 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 21:01:21 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 21:01:27 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 21:04:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 21:04:31 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 21:04:34 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 21:04:36 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 21:04:56 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 21:05:02 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 21:05:04 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 21:05:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 21:05:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb67fc22738d58442db1bd40a3c6f60cb5038ef87b356fda058eae811b9e66a1`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 1.7 MB (1744650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c452ba09cd632ffe58aa658dc18133d1783bb3b475ac3001e7cb6492a41dcb`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03960c8a570255096ca4926f8aac09cdf62550255cb84376f5dab02635482972`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccee9e2de6a3547aca22a73c28f0733f5208a257bc692dd73a26f26ace54e4c`  
		Last Modified: Tue, 05 Apr 2022 05:11:25 GMT  
		Size: 10.4 MB (10438294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5ecc38bce13b7829819048860d15c87c726f2b846aaddc25299933504cda2`  
		Last Modified: Tue, 05 Apr 2022 05:11:24 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f3ed5b861790de146d751f0e42d99f932070450c9055c3c05118c52b37a413`  
		Last Modified: Tue, 05 Apr 2022 05:12:25 GMT  
		Size: 12.2 MB (12151066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2773ea1975991b44b27f2bda3061af34e8dada743717b970cb5b5a7512917d35`  
		Last Modified: Tue, 05 Apr 2022 05:12:22 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c077b38315bb0a5a58a543311e47869cca4f472fa981b0e3ed6ff6ce93a3f7`  
		Last Modified: Tue, 05 Apr 2022 05:12:22 GMT  
		Size: 18.4 KB (18389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadc7731f224112c35875e0e247118a575f661739c9be587657f4221187e1765`  
		Last Modified: Tue, 05 Apr 2022 05:12:22 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a089752383a31f903ea31325d8c86246386fe7a86a73ac3b62b1a8ea497a621`  
		Last Modified: Tue, 05 Apr 2022 21:21:09 GMT  
		Size: 528.6 KB (528613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb21952abb76fea79fad8b666e1d93c8edd041b7fe45c25adb95037aed1343`  
		Last Modified: Tue, 05 Apr 2022 21:21:12 GMT  
		Size: 21.1 MB (21050463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca742a1ba6362914a295c4b539f4ffb7ff533679004532e8b7da877abf45d71`  
		Last Modified: Tue, 05 Apr 2022 21:21:13 GMT  
		Size: 22.3 MB (22344181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cd8054acafabd46d43a65de9dbb8292031349fb94c13afca38b73a0bfba4c0`  
		Last Modified: Tue, 05 Apr 2022 21:21:09 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff16a3502ca5013e78aef4d56b1198a5ed193e0d0276b93cf0380291a62c3b2a`  
		Last Modified: Tue, 05 Apr 2022 21:21:08 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:8df403aa8be07bf605926b725c8b090c5d7b13aa93a41955dc71e9dd882185e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69130159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d007c42ea0057ad08a621951632067b235cea77f86b8e300ed720c9e9d390e66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:02:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:02:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:02:59 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:02:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:03:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:42:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 00:42:26 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 00:42:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 00:42:26 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 00:42:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:42:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:47:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:47:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:47:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:47:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:47:57 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:47:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:47:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:47:57 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:47:58 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 12:23:29 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 05 Apr 2022 12:23:30 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 05 Apr 2022 12:23:31 GMT
RUN apk add --no-cache 	bash
# Tue, 05 Apr 2022 12:25:34 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		gmp-dev 		icu-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Tue, 05 Apr 2022 12:25:36 GMT
VOLUME [/var/www/html]
# Tue, 05 Apr 2022 12:25:36 GMT
ENV JOOMLA_VERSION=4.1.2
# Tue, 05 Apr 2022 12:25:37 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Tue, 05 Apr 2022 12:25:51 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Tue, 05 Apr 2022 12:25:55 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Tue, 05 Apr 2022 12:25:55 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Tue, 05 Apr 2022 12:25:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 05 Apr 2022 12:25:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df780ceebfdd113d5a6f5772c1d4abeb603e14b99c871ea2281632b11cf6f759`  
		Last Modified: Tue, 05 Apr 2022 01:09:34 GMT  
		Size: 1.8 MB (1760653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5640ab2fd0b3501350a8a837b003d809c84b6169e11a74c71e7a193175a3e3`  
		Last Modified: Tue, 05 Apr 2022 01:09:35 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910c970dadd8c90e6942fd635f2d508e9f2a2ecd4c5281578cf6470fa8bc432`  
		Last Modified: Tue, 05 Apr 2022 01:09:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80802a49593a51039cf00accf74acac1c125b0572abe00ced38a237f324507da`  
		Last Modified: Tue, 05 Apr 2022 02:55:03 GMT  
		Size: 10.4 MB (10438304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79bdfdd359a6b4ab77a6ee661b37b97a3b5cf10a4f381cda26358e1eb5a092d`  
		Last Modified: Tue, 05 Apr 2022 02:55:03 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107391fe7a9f3c9234e063411766652eec8b08c35703a04f9c2b0f161be8aa7b`  
		Last Modified: Tue, 05 Apr 2022 02:55:38 GMT  
		Size: 11.0 MB (11022313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40736353ed5fd5a3b6c1d31123697732c642edd46a6b1a1de7b4d3d9af3544a`  
		Last Modified: Tue, 05 Apr 2022 02:55:36 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5efefd9741c8d25fec55894a43249b1779c09dd33f6e592d155158e3f92e5f2`  
		Last Modified: Tue, 05 Apr 2022 02:55:36 GMT  
		Size: 18.4 KB (18414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcd94e8f7b4932ecc5b69eb12a211acda1f46e78a35a07d5a4e8caadcf1e1f8`  
		Last Modified: Tue, 05 Apr 2022 02:55:37 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf47d9e2cd1c9aa93e1de9391cb43d2271b07518bd7a9dc696d658c8488ea3f6`  
		Last Modified: Tue, 05 Apr 2022 12:36:40 GMT  
		Size: 483.4 KB (483428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666985bdd07e0334dee5ffa87adfc06a217a068d1ec37a9ff66b4e32eb26a8e6`  
		Last Modified: Tue, 05 Apr 2022 12:36:43 GMT  
		Size: 20.4 MB (20447141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc255eeebc1cc1f93df02dd7162bb76d760b1d14c4d1d1dba81669e9aa50046`  
		Last Modified: Tue, 05 Apr 2022 12:36:43 GMT  
		Size: 22.3 MB (22344180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c501b873bc4f251a598ead710355849a9a3972a2236c08f46bfd3e1253aeae5b`  
		Last Modified: Tue, 05 Apr 2022 12:36:40 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684e4e23e7134ae7313824ff7a85c55dfd15a67a6837adba5710208cbbc813bb`  
		Last Modified: Tue, 05 Apr 2022 12:36:41 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
