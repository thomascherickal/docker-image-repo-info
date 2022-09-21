## `drupal:php7.4-fpm-alpine`

```console
$ docker pull drupal@sha256:1fd64e4d36a0cd1ffab775f34310f64d8b93adab76ddeb70822bd381d0f89cda
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

### `drupal:php7.4-fpm-alpine` - linux; amd64

```console
$ docker pull drupal@sha256:b8035aff81b7644f4622b74c7544078d3406c531f88959a55eb46a1e01bca41e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (51014061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f364ed2add92bc3a65ebb5b67bde393c99067a5cd2c94dddd0e7af65cdf60a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:20:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 21:20:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 21:20:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 21:20:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 21:20:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 22:34:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Aug 2022 22:34:26 GMT
ENV PHP_VERSION=7.4.30
# Tue, 09 Aug 2022 22:34:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 09 Aug 2022 22:34:26 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 09 Aug 2022 22:34:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 09 Aug 2022 22:34:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Aug 2022 22:41:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Aug 2022 22:41:50 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 09 Aug 2022 22:41:51 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Aug 2022 22:41:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Aug 2022 22:41:51 GMT
WORKDIR /var/www/html
# Tue, 09 Aug 2022 22:41:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Aug 2022 22:41:52 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 22:41:52 GMT
EXPOSE 9000
# Tue, 09 Aug 2022 22:41:52 GMT
CMD ["php-fpm"]
# Wed, 10 Aug 2022 04:25:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 10 Aug 2022 04:25:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:46:22 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:36:41 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:36:41 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:36:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:36:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a600fdbc30cc6501babd12a4b22d75316d5ae384a68b9b4c588bfba33109bbc0`  
		Last Modified: Tue, 09 Aug 2022 23:00:27 GMT  
		Size: 1.7 MB (1720948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdd6cb15c0d57bb696f4a1a47b41374e78a6a5f1cdd24c45d8b9655b52caa40`  
		Last Modified: Tue, 09 Aug 2022 23:00:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c40d8aee7b41f415744811ec585376e2f7798b79ac68e04b7127fb847d566`  
		Last Modified: Tue, 09 Aug 2022 23:00:26 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e67522f4fd69104b389667cdaa7cbac2c77f9de63edb5cfb9ab7e672232186`  
		Last Modified: Tue, 09 Aug 2022 23:08:03 GMT  
		Size: 10.4 MB (10439251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d181492ef8e98df214123c11ce13997a4838a452a4e9f972b1f4398696d2b4d3`  
		Last Modified: Tue, 09 Aug 2022 23:08:02 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ee11034df499150189aac1cd6fd949decf096d76a6c9a12a0557e1766f2771`  
		Last Modified: Tue, 09 Aug 2022 23:08:43 GMT  
		Size: 11.5 MB (11456036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb72a5cacfff5d00259f42cffa0c125aae717fe8d31ce74971c690a8c67b16aa`  
		Last Modified: Tue, 09 Aug 2022 23:08:41 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acd67bcb441e4ae76c5e968ef8f59c4a1ca7db508f97e93b9317720d02bc94b`  
		Last Modified: Tue, 09 Aug 2022 23:08:41 GMT  
		Size: 18.6 KB (18620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9674ad94811d7edcb3760a26d8f2b7cf63e4e3986af550433d1277afdb57e`  
		Last Modified: Tue, 09 Aug 2022 23:08:41 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47203f389111e4a054f39a70474129614518feb1a7dc835c5106c32dd5b5b0c3`  
		Last Modified: Wed, 10 Aug 2022 04:39:16 GMT  
		Size: 2.0 MB (1991302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b1faa28bc0dbd70d7c83d0b3681b293c9980cffd04ec9909aad4cc54da262`  
		Last Modified: Wed, 10 Aug 2022 04:39:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b80d9f8cd8660faef8a5dcf46cad3bacd6773dc2d6c4987b3bab1cc308b8b23`  
		Last Modified: Mon, 22 Aug 2022 20:13:14 GMT  
		Size: 692.1 KB (692052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae87825fb95ec56a0f184f850b31fcfe834ef2c426a5c46b1fe610dd8edf62d3`  
		Last Modified: Tue, 20 Sep 2022 23:53:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e51cff4ad4bc9b75074cf8ea01a8e9d22905e11846ad93759b41e6c462513ed`  
		Last Modified: Tue, 20 Sep 2022 23:53:59 GMT  
		Size: 21.9 MB (21876406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull drupal@sha256:7a52b8301deb529896d42c523d1aadb61ea0d17f19b3acd5bdd725bed12693f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49892826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d9624eea6b706717d17081f1a86efbd4cbdb249455e798a8da1a9c913f655e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 11:16:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 11:16:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 11:16:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 11:16:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 11:16:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 15:06:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 10 Aug 2022 15:06:06 GMT
ENV PHP_VERSION=7.4.30
# Wed, 10 Aug 2022 15:06:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Wed, 10 Aug 2022 15:06:06 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Wed, 10 Aug 2022 15:06:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 15:06:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 15:29:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 15:29:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 10 Aug 2022 15:29:55 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 15:29:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 15:29:55 GMT
WORKDIR /var/www/html
# Wed, 10 Aug 2022 15:29:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 10 Aug 2022 15:29:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 10 Aug 2022 15:29:56 GMT
EXPOSE 9000
# Wed, 10 Aug 2022 15:29:56 GMT
CMD ["php-fpm"]
# Thu, 11 Aug 2022 01:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 11 Aug 2022 01:47:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:09:35 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:51:43 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:51:43 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:51:57 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:51:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6fa03280302058f33539e036c049c26e6b1f95d1306b571a247717725212b5`  
		Last Modified: Wed, 10 Aug 2022 16:20:51 GMT  
		Size: 1.7 MB (1707962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a0a3e2190be4d464337d2b34ae250925d898b9100464d1528683a35ea7b54d`  
		Last Modified: Wed, 10 Aug 2022 16:20:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb22106c208d7e172696b03b8551465117d04b728caffe704132bdf3246185`  
		Last Modified: Wed, 10 Aug 2022 16:20:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8986186cf3803bdff6640cfe7c826014b04619380d1bf6f4100fae7c7d008200`  
		Last Modified: Wed, 10 Aug 2022 16:29:35 GMT  
		Size: 10.4 MB (10439247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb88e6290a119ca5e77c53f6d494a6921fe39b4d2e8c891ec1dfc3532fc9f96d`  
		Last Modified: Wed, 10 Aug 2022 16:29:33 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f9b42798deef2716dd601c0122177bf0834490d3f0d62b0a09c674373725fc`  
		Last Modified: Wed, 10 Aug 2022 16:30:29 GMT  
		Size: 10.7 MB (10722959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebffeb27ef4d496f390be033e38a4e2a929fefc00fc6e265276837cbdfe9a9d`  
		Last Modified: Wed, 10 Aug 2022 16:30:25 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33391253c87d17212f14886db4776a96df70a0ce8f24754e3e78bb416a85c68e`  
		Last Modified: Wed, 10 Aug 2022 16:30:25 GMT  
		Size: 18.6 KB (18634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a88ec008d323e42904d4ef3c6782f499b6fbe7f9da85900837313da12e2c69`  
		Last Modified: Wed, 10 Aug 2022 16:30:25 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43840d7447f0b177e9795dc9838a1a6ea60676141f411686bc9328943b99a06f`  
		Last Modified: Thu, 11 Aug 2022 02:00:55 GMT  
		Size: 1.8 MB (1808266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f418d7a29da6b8b0bd0496eba4d646eae9a63c77bdfe3f0165576bae3c7c83`  
		Last Modified: Thu, 11 Aug 2022 02:00:55 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af721e66eca61a97a66deebf9d987c13bf5621368f22d6dbeac0af701f10c442`  
		Last Modified: Mon, 22 Aug 2022 19:22:41 GMT  
		Size: 692.1 KB (692057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0efa1008a5a321689134ec0cc4057b593c713f6c11877895f065a12e2e68d6`  
		Last Modified: Wed, 21 Sep 2022 00:01:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f7632fb818ebb17c912c31ad315ad93f68396cfe5934ec4349a043e5b9fc7c`  
		Last Modified: Wed, 21 Sep 2022 00:01:24 GMT  
		Size: 21.9 MB (21876347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull drupal@sha256:043293f5bb978562bd87bf16e967aa40c1c9037ac12b2fce99ef320e463ae22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48773539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89e352d5615e0c1c8f40b385effdd23ae7d4d304aa5eb2a353678c27adf70110`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 14:13:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 14:13:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 14:13:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 14:13:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 14:13:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 17:55:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 10 Aug 2022 17:55:24 GMT
ENV PHP_VERSION=7.4.30
# Wed, 10 Aug 2022 17:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Wed, 10 Aug 2022 17:55:24 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Wed, 10 Aug 2022 17:55:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 17:55:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 18:19:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 18:19:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 10 Aug 2022 18:19:24 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 18:19:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 18:19:24 GMT
WORKDIR /var/www/html
# Wed, 10 Aug 2022 18:19:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 10 Aug 2022 18:19:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 10 Aug 2022 18:19:25 GMT
EXPOSE 9000
# Wed, 10 Aug 2022 18:19:25 GMT
CMD ["php-fpm"]
# Thu, 11 Aug 2022 05:08:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 11 Aug 2022 05:08:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:29:03 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Wed, 21 Sep 2022 00:08:27 GMT
ENV DRUPAL_VERSION=9.4.6
# Wed, 21 Sep 2022 00:08:27 GMT
WORKDIR /opt/drupal
# Wed, 21 Sep 2022 00:08:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 21 Sep 2022 00:08:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533661cc695e850f2ce9a61f8d6bcabf20631bc4be493498e7c06a85445a834d`  
		Last Modified: Wed, 10 Aug 2022 19:17:39 GMT  
		Size: 1.6 MB (1575470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ea8309925b47b4d8ed5708b410d6856267d8d8dea3544802ae2a6d8e16e2a5`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a23ce236c2c67c8bab1a6d9e5111a49299c4b7a07b9914b84c845eb1ff3c3ab`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631888119424639e4b242212cc3f458f767eb7c9c2d2ca5956ee4868fc4e1d7`  
		Last Modified: Wed, 10 Aug 2022 19:27:59 GMT  
		Size: 10.4 MB (10439228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bf5933f24fe516c25b89b8912e9c3bd5a3a9aa5117a389b1207f5795e7dd62`  
		Last Modified: Wed, 10 Aug 2022 19:27:58 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595ade0f864be84f642c42d32af421c096576e17761bd9193055408f8d3c750d`  
		Last Modified: Wed, 10 Aug 2022 19:28:53 GMT  
		Size: 10.1 MB (10089555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15716a97078c814bfc08d7d1bae3a309f048158c7ec7fb5f30809d064a8dad`  
		Last Modified: Wed, 10 Aug 2022 19:28:49 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c23b12efd1cf56383e5343780a9a21fc78936fc7ddee7e89cb363a2e9ed2cd`  
		Last Modified: Wed, 10 Aug 2022 19:28:48 GMT  
		Size: 18.6 KB (18609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdba9263d658accf7dbd171fc652cce1956e6999ea02542337ee19165b893252`  
		Last Modified: Wed, 10 Aug 2022 19:28:49 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fe20e3720a1aae5d23d934e53347120b3f9a7de6f7eee99755af10622a0652`  
		Last Modified: Thu, 11 Aug 2022 05:34:41 GMT  
		Size: 1.7 MB (1653360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90aad4216da0b5b2e2f81096f11396e5450255bcdc7e451b3e905e4ee776934c`  
		Last Modified: Thu, 11 Aug 2022 05:34:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca916eca2ea89011abb3f2aa09b637e6bfe765ee8a36bc7702c20b2d1c449488`  
		Last Modified: Mon, 22 Aug 2022 20:13:05 GMT  
		Size: 692.0 KB (692047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccedbe2dabbc32f682dc7650834b54f80ca35917de30774f9e80fe0f8b0f6ca4`  
		Last Modified: Wed, 21 Sep 2022 00:40:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dfdef4a59fa6694f35997c8c275f8a7471ea4d8a7bbdb03e63c009f3b04219`  
		Last Modified: Wed, 21 Sep 2022 00:40:39 GMT  
		Size: 21.9 MB (21874812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:d8d093df6524606d94812c9c8cde7f3d908ad14a6bfcade50e402a7403302931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50687546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e355c83c6722cacf6a423ed3b7a55aa0fa186285e6143375de1472c0e05e0cfd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:03:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 00:03:59 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 00:04:00 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 00:04:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 00:04:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 00:04:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:04:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:04:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 01:42:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 10 Aug 2022 01:42:12 GMT
ENV PHP_VERSION=7.4.30
# Wed, 10 Aug 2022 01:42:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Wed, 10 Aug 2022 01:42:14 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Wed, 10 Aug 2022 01:42:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 01:42:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 01:50:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 01:50:05 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 10 Aug 2022 01:50:06 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 01:50:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 01:50:07 GMT
WORKDIR /var/www/html
# Wed, 10 Aug 2022 01:50:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 10 Aug 2022 01:50:09 GMT
STOPSIGNAL SIGQUIT
# Wed, 10 Aug 2022 01:50:10 GMT
EXPOSE 9000
# Wed, 10 Aug 2022 01:50:11 GMT
CMD ["php-fpm"]
# Wed, 10 Aug 2022 07:26:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 10 Aug 2022 07:26:22 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:09:53 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:52:47 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:52:48 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:53:04 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:53:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2451bb80cc25fd19497adebf3450060e0befb8338668e6f8f8997c1cdbfa8449`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 1.7 MB (1715287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8596f4ed07f5a52b53624b796113b36143107921db4f999141aeaf08e9726c`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753cf0136f4270e91e1fcba1ad4b3a086700d0092f3fd518f573ee69444de99d`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383263d48dfcb9b7c08feb71d0afcb56efd230f30152447a94c3fc7aa705e356`  
		Last Modified: Wed, 10 Aug 2022 02:23:32 GMT  
		Size: 10.4 MB (10439022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632eebe9780d968946c6e0182c33b2c58a249d097fa16cf7191ea925b65c5ac5`  
		Last Modified: Wed, 10 Aug 2022 02:23:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21819b644174948a34e6c694f939830d1cdbac0881c3d81d242c006c40d3471c`  
		Last Modified: Wed, 10 Aug 2022 02:24:22 GMT  
		Size: 11.3 MB (11284205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd35e5c69ada77c3ad46dc7a16b49154fcc9fe7599249dec25d5bb7c7f612187`  
		Last Modified: Wed, 10 Aug 2022 02:24:20 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a81f51d2d5b99a875d3b281a551fa8c1df8624e6c5d0fb0ab0ca5aaf0933c24`  
		Last Modified: Wed, 10 Aug 2022 02:24:21 GMT  
		Size: 18.5 KB (18535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bff46c3a926d34a356560b6a0f44d96a9785a36e7c8f683865aec2bb94e991a`  
		Last Modified: Wed, 10 Aug 2022 02:24:20 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390fc7fec341ec3a8091333b8f5fa82829264c040befc9e4f018aeed7995905`  
		Last Modified: Wed, 10 Aug 2022 07:48:54 GMT  
		Size: 1.9 MB (1939650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a976638fe28e2a2db9f6e12a3be4637839aa2d8ccf4b9b3cb42b5936957504`  
		Last Modified: Wed, 10 Aug 2022 07:48:53 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaf1868b888dd72e50ca80626684488ee96cd45aa01caa38229ab2493de6f18`  
		Last Modified: Mon, 22 Aug 2022 19:47:03 GMT  
		Size: 692.1 KB (692052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913596254730f6dc55391c27f0bc96229da3003723559e1785b22a87797b0911`  
		Last Modified: Wed, 21 Sep 2022 00:19:00 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1427816f99ad03171ed870764a4583a4c784503ec80f90a09f2515d2a3f932c`  
		Last Modified: Wed, 21 Sep 2022 00:19:05 GMT  
		Size: 21.9 MB (21877852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; 386

```console
$ docker pull drupal@sha256:ef901fede3cb3dfc4c0af9cf78d085f97d50a618f9847946f3dbbaf71dbe8a72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51518680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59a4229fe2bb82cb4ee9536291e7502da9ffa6f05f09cd4d0147d0636d6dd57c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:56:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 18:56:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 18:56:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 18:56:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 18:56:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 18:56:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 18:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 18:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 20:10:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Aug 2022 20:10:08 GMT
ENV PHP_VERSION=7.4.30
# Tue, 09 Aug 2022 20:10:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 09 Aug 2022 20:10:10 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 09 Aug 2022 20:10:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 09 Aug 2022 20:10:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Aug 2022 20:17:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Aug 2022 20:17:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 09 Aug 2022 20:17:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Aug 2022 20:17:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Aug 2022 20:17:38 GMT
WORKDIR /var/www/html
# Tue, 09 Aug 2022 20:17:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Aug 2022 20:17:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:17:41 GMT
EXPOSE 9000
# Tue, 09 Aug 2022 20:17:42 GMT
CMD ["php-fpm"]
# Wed, 10 Aug 2022 01:47:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 10 Aug 2022 01:47:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:06:30 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:47:45 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:47:46 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:48:01 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:48:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a15900474f3d2d2c9944341ff070dc1daf50815820580bd21463737a6c55a`  
		Last Modified: Tue, 09 Aug 2022 20:41:11 GMT  
		Size: 1.8 MB (1820367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40080bc9e2b22eebc8070ba53b95939ccd7e292319817fbcd98639a046e4da31`  
		Last Modified: Tue, 09 Aug 2022 20:41:11 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e6830783d889ccc83e35eab559566fe80ed99bf0d67035474ed38e5ddc7b02`  
		Last Modified: Tue, 09 Aug 2022 20:41:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9290da3bc94d7c9f83a5a9f4cfafb91a5f90d42a8a047190fce9b6be1416d60`  
		Last Modified: Tue, 09 Aug 2022 20:50:24 GMT  
		Size: 10.4 MB (10439012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8210997aeb06ce66209b417c92c83fe45fd2d4e3bb3a2a5e9fba7d4eae907`  
		Last Modified: Tue, 09 Aug 2022 20:50:22 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45728acf4b6f616545c7f330b12b75721dc224a34b9b801ceef0f694abc99ecf`  
		Last Modified: Tue, 09 Aug 2022 20:51:11 GMT  
		Size: 11.8 MB (11764720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bb1e3cb7a801f05f8c12a02b2cc02593bb64b582b6cf1e325f5b397b6a9b7f`  
		Last Modified: Tue, 09 Aug 2022 20:51:09 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fed0805de402895a959387cf2e77722a858bbde022df8479afb37d2c27b7b1`  
		Last Modified: Tue, 09 Aug 2022 20:51:09 GMT  
		Size: 18.5 KB (18516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9695ba6fa36cd59a08232357c7091fd48a6aba5d079993bd5d2c9d8a0997c1`  
		Last Modified: Tue, 09 Aug 2022 20:51:09 GMT  
		Size: 8.4 KB (8437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51189e43cef49d7bea0580ad361bdc0afaf65fb9692fb960b8f31cf896e41bcd`  
		Last Modified: Wed, 10 Aug 2022 02:10:39 GMT  
		Size: 2.1 MB (2085353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f41d82ca1e977b2b2ea57f0af3221676a24b2bb1a7adfa119986029d817dca`  
		Last Modified: Wed, 10 Aug 2022 02:10:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4b690a940223ced56ee2aa516b274a454463d6ac839336ac79a113a8eb31c3`  
		Last Modified: Mon, 22 Aug 2022 19:43:39 GMT  
		Size: 692.1 KB (692055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dccc507a17f0132cc7393356c1f2982da1f72e0b372e5883b0a39a0b5937bff`  
		Last Modified: Wed, 21 Sep 2022 00:15:00 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613ed5823211986b6aaf3e1b349ee0e975ec6b62fd6b0e835dcc2775bbfa0e20`  
		Last Modified: Wed, 21 Sep 2022 00:15:05 GMT  
		Size: 21.9 MB (21878264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; ppc64le

```console
$ docker pull drupal@sha256:ede0da9dfd6b2536f1731f365949742cf5d3c1f58ba5ffe222cdde4e37033fe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51928785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31307596453af68ddbb6015f807961e2fe9bcf21c7d5b4bbcf2567bf61001127`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:38:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 19:38:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 19:38:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 19:38:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 19:38:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 19:38:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:38:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:38:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 21:17:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Aug 2022 21:17:33 GMT
ENV PHP_VERSION=7.4.30
# Tue, 09 Aug 2022 21:17:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 09 Aug 2022 21:17:34 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 09 Aug 2022 21:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 09 Aug 2022 21:17:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Aug 2022 21:27:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Aug 2022 21:27:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 09 Aug 2022 21:27:29 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Aug 2022 21:27:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Aug 2022 21:27:30 GMT
WORKDIR /var/www/html
# Tue, 09 Aug 2022 21:27:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 09 Aug 2022 21:27:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 21:27:33 GMT
EXPOSE 9000
# Tue, 09 Aug 2022 21:27:33 GMT
CMD ["php-fpm"]
# Wed, 10 Aug 2022 07:29:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 10 Aug 2022 07:29:37 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:50:03 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:25:43 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:25:44 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:26:10 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:26:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b19bea03a0d19d92d9affb999a9d6e5bddf7ccb99ced434a118735e98eda42`  
		Last Modified: Tue, 09 Aug 2022 21:56:16 GMT  
		Size: 1.8 MB (1772201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9859feb1e3bcc24ef58fc12055cdbc53accb9d3c77721c61161ec83fd7cfb6`  
		Last Modified: Tue, 09 Aug 2022 21:56:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c00a2acb11c8adb08413d315161b5e31709b25d4a157a151371861eaca20fd9`  
		Last Modified: Tue, 09 Aug 2022 21:56:15 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8603160e8827c3b805bce01160750a8b8f1043a747a289f00afbcd1838575b`  
		Last Modified: Tue, 09 Aug 2022 22:06:52 GMT  
		Size: 10.4 MB (10439253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07870f7acd7cdc93e72514687cd9397b560cbeec28de94f445b4f11ff23da795`  
		Last Modified: Tue, 09 Aug 2022 22:06:51 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fa02d2b73dedccb5aac1152f39dc8e70c91558ff995b7f2341b7790519dfbf`  
		Last Modified: Tue, 09 Aug 2022 22:07:52 GMT  
		Size: 12.2 MB (12217182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84afdd499c2b616e95fd17164245c851d189f7085a6d950760edec3712d95b9d`  
		Last Modified: Tue, 09 Aug 2022 22:07:48 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0ff7507cd63cc4e8b0459ce58696d6b686f4866c79c1c1ab2305697df88a5f`  
		Last Modified: Tue, 09 Aug 2022 22:07:49 GMT  
		Size: 18.6 KB (18620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4354b14d540b5c726e7ac04d349da5f6017af0b7bce772b2ad640df84ab93f20`  
		Last Modified: Tue, 09 Aug 2022 22:07:49 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076c1c57e9d752ef1a972570808b0c9bddb9e4f907b628fd9226378aa5fceb99`  
		Last Modified: Wed, 10 Aug 2022 07:56:57 GMT  
		Size: 2.1 MB (2096135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86679c59ffec49fd83f00b4b90e3dca2b62ddc391ff89ad245f2ce9eb662c519`  
		Last Modified: Wed, 10 Aug 2022 07:56:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ed17b04cfab5cddf4049ac8c088dae316ac2d831494ce9b14c6282de9fd8cb`  
		Last Modified: Mon, 22 Aug 2022 20:39:02 GMT  
		Size: 692.1 KB (692053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2e91f66abca1c8ea6977217c29009cce15deefd1e44b25c99bc0eb0537660f`  
		Last Modified: Tue, 20 Sep 2022 23:50:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db0cf6cef4f1def95fd901a5dff1cae2dfe26a3298e0c7650187b0eb04082bf`  
		Last Modified: Tue, 20 Sep 2022 23:50:24 GMT  
		Size: 21.9 MB (21876628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine` - linux; s390x

```console
$ docker pull drupal@sha256:6f8f51baccc34fbc954ccf40c07225c72b0505be149459d14bbbaacd6d38366d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50422696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f098877cd4489e1268fef3e3afa54e272dba7663336251ccf286375cbd749a02`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:13:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 23:13:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 23:13:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 23:13:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 23:13:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 00:40:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 10 Aug 2022 00:40:02 GMT
ENV PHP_VERSION=7.4.30
# Wed, 10 Aug 2022 00:40:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Wed, 10 Aug 2022 00:40:03 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Wed, 10 Aug 2022 00:40:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 00:40:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:48:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 00:48:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:48:39 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 00:48:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 00:48:39 GMT
WORKDIR /var/www/html
# Wed, 10 Aug 2022 00:48:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 10 Aug 2022 00:48:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 10 Aug 2022 00:48:40 GMT
EXPOSE 9000
# Wed, 10 Aug 2022 00:48:40 GMT
CMD ["php-fpm"]
# Wed, 10 Aug 2022 11:02:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 10 Aug 2022 11:02:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 22 Aug 2022 19:12:03 GMT
COPY file:4d0825f63a9e599415e16f45e6edd9174543d5a1499166c8c1dd3050562baaf5 in /usr/local/bin/ 
# Tue, 20 Sep 2022 23:51:24 GMT
ENV DRUPAL_VERSION=9.4.6
# Tue, 20 Sep 2022 23:51:25 GMT
WORKDIR /opt/drupal
# Tue, 20 Sep 2022 23:51:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 20 Sep 2022 23:51:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c93f21d9f546f68476c05adafca1709482765850b132881bc932f21c2c4a22`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 1.8 MB (1775799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3435c93d9a06d643ccde0e4d6a2f2e1352451f34309ec4c24470974d6ed10d7`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe8bd3886087a99fec0c70835271597facb70fc1e142318fef69263a4b277d4`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f1b78caec4c3065bea94e7c3028757fcee4f42b416d7465e42cea5c866894c`  
		Last Modified: Wed, 10 Aug 2022 02:14:57 GMT  
		Size: 10.4 MB (10439260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932d4c6d074ed3502da6095000baab6e99eff1860b202742312d0fd006da5e25`  
		Last Modified: Wed, 10 Aug 2022 02:14:57 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1d6b4f24a71485e34023da9e46cf2feec9dc2b87234cef25cdf6ac4205a21d`  
		Last Modified: Wed, 10 Aug 2022 02:22:34 GMT  
		Size: 11.1 MB (11050061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f330909a34a400f799831c5babd268180aee902b8e802b034d9c226c3e9cc3`  
		Last Modified: Wed, 10 Aug 2022 02:22:34 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5d4e610e79c70d9f8d208ff1bc81e63546a8dfe797aa67e3b386c045ea7ab3`  
		Last Modified: Wed, 10 Aug 2022 02:22:34 GMT  
		Size: 18.6 KB (18638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a824a97db9867d4dc1f3c35bf146b1448f354ab915988d686f1209f6ec74895`  
		Last Modified: Wed, 10 Aug 2022 02:22:34 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be67f852a5113a4dd4ec76080e793b968d995bdb76f72d99f8c830f2c23e2981`  
		Last Modified: Wed, 10 Aug 2022 12:04:35 GMT  
		Size: 2.0 MB (1969904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34469e628f727698d6c7e91c500c55e7a2f8b3a5ca907d2be621ef7240a61779`  
		Last Modified: Wed, 10 Aug 2022 12:04:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa60cbd4f4e981ba3949e703448422a5906fc0bec75566590dbe3f9f2e8400`  
		Last Modified: Mon, 22 Aug 2022 19:43:28 GMT  
		Size: 692.1 KB (692053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e62172159a365eb6d588dc75e0d829e67f7e6de7cac88e5d4a19293db21052`  
		Last Modified: Wed, 21 Sep 2022 01:28:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf93e8adb107f51778a9a2635dce49c5b6a356b488ecf837a6af5e6a549aead`  
		Last Modified: Wed, 21 Sep 2022 01:28:39 GMT  
		Size: 21.9 MB (21872991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
