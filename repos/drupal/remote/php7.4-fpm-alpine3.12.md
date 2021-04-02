## `drupal:php7.4-fpm-alpine3.12`

```console
$ docker pull drupal@sha256:99cea3afa93db1459a458173876f93e96bc90a851a10e2fabfd1990146bfef33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:php7.4-fpm-alpine3.12` - linux; amd64

```console
$ docker pull drupal@sha256:e74d538ff9e022c10316937ce6527541da3f2c12f47ec448cbb39c6824b02cdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (51043852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5940f9bcc6bd448dba3a85165779a1030fbcfada0bcdeb2007b699d5eaafaf59`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 15:35:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 15:35:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 15:35:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 15:35:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 15:35:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 16:07:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 16:07:32 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 16:07:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 16:07:32 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 16:07:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 16:07:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 16:12:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 16:12:01 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 16:12:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 16:12:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 16:12:03 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 16:12:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 16:12:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 16:12:04 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 16:12:05 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 19:30:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 19:30:23 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 20:49:13 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 20:49:14 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 20:49:14 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 20:49:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 20:49:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff8d50decdf72ea74c5f261dc5027350a4d32b7c326e4696042548e89a9cf1`  
		Last Modified: Thu, 01 Apr 2021 16:53:59 GMT  
		Size: 1.3 MB (1340902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a17e65b2c2a5419af1354742266ba010b1f9274700addf98c557da542df413b`  
		Last Modified: Thu, 01 Apr 2021 16:53:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5babbc773bdaab8d8228e4ea1eb6a10e9e7d62e48fff14cf0d90914bace56cf`  
		Last Modified: Thu, 01 Apr 2021 16:54:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42327044be6d1f99b07059660a3574fa271bbf53cca040ef144a7ba741221aca`  
		Last Modified: Thu, 01 Apr 2021 16:57:13 GMT  
		Size: 10.4 MB (10353552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f752747adee01fb9c1e6ec79236aba2c24a001664ef0199e392847405d31c69`  
		Last Modified: Thu, 01 Apr 2021 16:57:10 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab79590fe2692c4b74b6c8a28ca93188fa41579490c635caf28ec18625dbb5b`  
		Last Modified: Thu, 01 Apr 2021 16:57:13 GMT  
		Size: 14.3 MB (14278098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f39c1ec2f8d7c2d8f65625b46b0984b488e8b91c682dc013c1e8fbdd1fba383`  
		Last Modified: Thu, 01 Apr 2021 16:57:10 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9556be4e2417c6ca4e5ac5367c6798146e9b88f4e5e1e0a2f773c55a85de95fe`  
		Last Modified: Thu, 01 Apr 2021 16:57:10 GMT  
		Size: 16.9 KB (16888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a16f9b8c9d5ee72b5fae7943a7a7072ac34e85fa65c05fd5ad683bd896ec47`  
		Last Modified: Thu, 01 Apr 2021 16:57:10 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2769ad23db662c19c8d2e737bd875dc4268ee0d5ebd50fa29c990cf369aab810`  
		Last Modified: Thu, 01 Apr 2021 19:36:41 GMT  
		Size: 2.9 MB (2861196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ea84e5ddfcd5a7369a6c016b5f1a67696087e5ca72c44462fb7539b41413bc`  
		Last Modified: Thu, 01 Apr 2021 19:36:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736084bb284b3e881339b7a870c93baca3508dd93a0a88fd48d7f6943a4fc025`  
		Last Modified: Thu, 01 Apr 2021 21:01:52 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc77a00b0515f6e0cd9536743d48773910f35f36b7552d9ef22e79db3ff3cab`  
		Last Modified: Thu, 01 Apr 2021 21:01:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609f4bdf2e777b44c0229c4f1dbbb7561ab575f9a05d2d82565818cff60d88c0`  
		Last Modified: Thu, 01 Apr 2021 21:01:57 GMT  
		Size: 18.8 MB (18827289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm variant v6

```console
$ docker pull drupal@sha256:346d30e4f66fc88cba7b91c36ef46b8f7607cbf0339c91c28b3fdca6bcc2f218
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49698591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ce546da3836c44e3f544f3ec7a07b44d8ee7d6a132d1373e1c702ec0c67a06`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:47:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 31 Mar 2021 22:47:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 31 Mar 2021 22:47:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 31 Mar 2021 22:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 22:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 22:54:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 22:54:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:54:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:54:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 23:20:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 23:20:25 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 23:20:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 23:20:28 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 23:20:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 23:20:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:24:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 23:24:36 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:24:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 23:24:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 23:24:45 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 23:24:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 23:24:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 23:24:50 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 23:24:51 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 05:20:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 05:20:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:07:01 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:07:04 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:07:04 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:07:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:07:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c015d2eaf8e9ab8eacefeae519999e683b3a0ed18a191adb3a65a562ce8eb`  
		Last Modified: Thu, 01 Apr 2021 00:03:16 GMT  
		Size: 1.3 MB (1310217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b442c2bebdb19fcc3177f200ff8ae47793c870b284148b7ae3d32e4b7d1cb0`  
		Last Modified: Thu, 01 Apr 2021 00:03:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d9a8d897698cf053dbf182ba7fd6339c136e27795724845908701a3b49aa6f`  
		Last Modified: Thu, 01 Apr 2021 00:03:14 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d80530cb783f013330db0dcf816e648dcc6001583cfbd053c4a495ee64ba6b`  
		Last Modified: Thu, 01 Apr 2021 00:06:14 GMT  
		Size: 10.4 MB (10353564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbb9a9971fd28caef5938353810579cbaf415654d4f3b4c41a58ec58c5e0935`  
		Last Modified: Thu, 01 Apr 2021 00:06:12 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bf96b647ac18ff9709bd25fec6150038001bddbda22d09b748ca8c6dd756f0`  
		Last Modified: Thu, 01 Apr 2021 00:06:16 GMT  
		Size: 13.3 MB (13289646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4355e094e660e1b811f19f1926b0111813fadce6bf442b8b0d5a550160d2971d`  
		Last Modified: Thu, 01 Apr 2021 00:06:12 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a909cbfdfd1b25f764b12abba405bb07d66d9aaf33b4feb34c6a10aa06396418`  
		Last Modified: Thu, 01 Apr 2021 00:06:12 GMT  
		Size: 16.9 KB (16885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ab705ef7b17b34b3913829b94ae7abea5bdb39c6561cd028a420a95fa8143a`  
		Last Modified: Thu, 01 Apr 2021 00:06:12 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a871333f64a9c6cbde9be4d2ee48e7469f8a23006bf17e6c384e377e3e63ebc`  
		Last Modified: Thu, 01 Apr 2021 05:24:48 GMT  
		Size: 2.7 MB (2730461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc23e941cd6e134286eddbf12bd71d6bc153bc843ee63956341083692395aec2`  
		Last Modified: Thu, 01 Apr 2021 05:24:47 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c49e2ffedbe1cd432847ab30df61e971ba493f63076fca1cab27835b537f328`  
		Last Modified: Thu, 01 Apr 2021 19:12:00 GMT  
		Size: 553.0 KB (553012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04668e2f68c683b355e7ead7251464a1495379ba29fb1906859a79d7ba7c01ce`  
		Last Modified: Thu, 01 Apr 2021 19:11:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3443931e3019770f3eced05106e794e2133d273b20e43eb1ebef7882a9ad05`  
		Last Modified: Thu, 01 Apr 2021 19:12:13 GMT  
		Size: 18.8 MB (18826944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm variant v7

```console
$ docker pull drupal@sha256:4d9395bc54f520aacac189f78ef84ba131648c0460037a066cce2d2ebf5ebd98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48305499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98d37302afc32aa675cbc3833f21394a610023a40c9d97452508056e5381e147`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:37:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 10:37:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 10:38:05 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 10:38:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 10:38:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 10:41:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 10:41:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:41:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:41:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 10:58:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 10:58:34 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 10:58:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 10:58:37 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 10:58:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 10:58:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 11:01:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 11:01:14 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 11:01:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 11:01:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 11:01:22 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 11:01:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 11:01:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 11:01:33 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 11:01:35 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 15:23:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 15:23:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:49:50 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:49:52 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:49:53 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:50:34 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:50:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014c2a1c880d4c4829e5eaf7cf0ec560d6196afc6217656cc6de4c4e133a607`  
		Last Modified: Thu, 01 Apr 2021 11:29:22 GMT  
		Size: 1.2 MB (1214329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acd9f9112566d47aee3c66982e8b96e01743dbfdf373e19aedff96dc560d782`  
		Last Modified: Thu, 01 Apr 2021 11:29:25 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817d5333294d06a092009820dfa37d07ff76bc101437d4c10f617903b8ebd070`  
		Last Modified: Thu, 01 Apr 2021 11:29:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b5a2d6b052f9ddb9c975498ddbc11d85fc83bac811ae664f9ff1f3e0a4a46f`  
		Last Modified: Thu, 01 Apr 2021 11:31:41 GMT  
		Size: 10.4 MB (10353552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5da698945ceb700edcbebc791660818158bb3a6b409662abb1d34adbdec90aa`  
		Last Modified: Thu, 01 Apr 2021 11:31:41 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3edb6bbf33414e55e4dd2fb164b0b9e065b80cd62a6b89d12ae3d0b62349a8a`  
		Last Modified: Thu, 01 Apr 2021 11:31:42 GMT  
		Size: 12.4 MB (12441420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeb6e699986ae70656108f01a9380bdfd7803763c6cb6b1cd1c7e3642ce839d`  
		Last Modified: Thu, 01 Apr 2021 11:31:38 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b06b6c869ac214589a9dcf7ac0c3ae11ef7b6d5bd59b27159961c9885693bb`  
		Last Modified: Thu, 01 Apr 2021 11:31:38 GMT  
		Size: 16.9 KB (16867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd6321addabecbf78d021cb8a2c86e29d0fa0bdf111e2293ce7136db8813de`  
		Last Modified: Thu, 01 Apr 2021 11:31:42 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e03f2e7a6bf5d80b99fc3a5eb54ac124ba1d721dd169b68a1e8c11cf8c934c5`  
		Last Modified: Thu, 01 Apr 2021 15:31:25 GMT  
		Size: 2.5 MB (2477410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9c89d11bfa81e11d036e00024adcaaff7be495ac827d3c03ca242a86b1ca2d`  
		Last Modified: Thu, 01 Apr 2021 15:31:24 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cfafa02b4d5fc8735b98415190e3a35bcdfd80a9acb8a695c5f788efe2b8db`  
		Last Modified: Thu, 01 Apr 2021 20:06:20 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efeec90dcd83c47295d0d6ff42ff2b5c9d62f6b78d4bb2afe02a58d6318e8e6d`  
		Last Modified: Thu, 01 Apr 2021 20:06:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ded6230cc08a624700156140e7b55e09d6a4ff742d8763b4077e1ac62aaa695`  
		Last Modified: Thu, 01 Apr 2021 20:06:32 GMT  
		Size: 18.8 MB (18827428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:4c4904c281931ffaa5e23c31d1b15eee267327c65452a0f3d41ebefdf16aa256
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50768648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d28cba1b8d4c8772346697a8ac4ca63f380948e894c4d3c2e16af7ca3ccf64b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:27:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 14:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 14:27:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 14:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 14:27:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 14:31:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 14:31:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:31:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:31:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 14:53:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 14:53:18 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 14:53:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 14:53:20 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 14:53:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 14:53:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:56:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 14:56:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:56:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 14:56:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 14:56:54 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 14:56:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 14:57:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 14:57:02 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 14:57:03 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 19:38:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 19:39:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:39:06 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:39:07 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:39:08 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:39:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:39:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dba67ea2fd5816dd837ab3462f2eb2eaa8f5b1de107ec82c8825805955830c`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 1.3 MB (1342973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84790c433c4c7efb40e084d3fff815c4bc175c07e527e3fc6103758d5118dd4`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed570efd768c764ea5c77c43a405863ea75c89092d334a29d0644c807e4798c8`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d37dd18a136930e5227f94b139a6c19f4b313eef40de00d7e24ce74bf20314`  
		Last Modified: Thu, 01 Apr 2021 15:31:26 GMT  
		Size: 10.4 MB (10353547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7dbf624d10fec3d84531f86adefda88bdbdb4116b6a4a171a92aaa6cb2a227`  
		Last Modified: Thu, 01 Apr 2021 15:31:22 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc402f63d89a4548e7bd0169b4f06e1c4813a0e15ba5f494f0bc9e75df917ae`  
		Last Modified: Thu, 01 Apr 2021 15:31:26 GMT  
		Size: 14.1 MB (14080317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21525fad90683216302e4e9df6329749f516900b6d3ec6bd93daf48516d58527`  
		Last Modified: Thu, 01 Apr 2021 15:31:23 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055efe1d5906dddcaa79eba6c9d933a9abe3719db10365e5018c585780e382ef`  
		Last Modified: Thu, 01 Apr 2021 15:31:23 GMT  
		Size: 16.9 KB (16882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60f03097e9a957980839051e95d17cd5ac353eec460250c545a7f6fc98bfdf9`  
		Last Modified: Thu, 01 Apr 2021 15:31:23 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05bf39d81e2bd2a99c7b41b7fabbdcd95246f70587fa40cfbc28f7ae31ed219`  
		Last Modified: Thu, 01 Apr 2021 19:51:40 GMT  
		Size: 2.9 MB (2871945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f9b83b4336ec24221ab3e1be1bd02b7d6d4dbb7ca16d76e2aa64cf93561c00`  
		Last Modified: Thu, 01 Apr 2021 19:51:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeb588b20652e86380d46ccefd9a64ebc79ebddfd8e88eb6a90de9b3a5339da`  
		Last Modified: Thu, 01 Apr 2021 19:51:39 GMT  
		Size: 553.0 KB (553009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea828abbb70399d7c9bfb8a1ea875622c83218f835297083b154d3fb978f18c`  
		Last Modified: Thu, 01 Apr 2021 19:51:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1d8be9dc7391eefdc9aa1e91a37494d5901ec3665726d35e5416636d9ae642`  
		Last Modified: Thu, 01 Apr 2021 19:51:49 GMT  
		Size: 18.8 MB (18826917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; 386

```console
$ docker pull drupal@sha256:8e2c09d901ec46f72be6cb33e6a798608891bc094df4216dee4fffc8b36327a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51715596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6501458f81fa029c26f163a9a7393cb1dc1a6c0fe74f64c07525d201ee0050e7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:02:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 03:02:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 03:02:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 03:02:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 03:02:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 03:41:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 03:41:59 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 03:41:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 03:41:59 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 03:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 03:42:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:47:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 03:47:45 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:47:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 03:47:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 03:47:47 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 03:47:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 03:47:48 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 03:47:48 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 03:47:49 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 09:20:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 09:20:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 18:57:40 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 18:57:41 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 18:57:41 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 18:57:54 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 18:57:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca80016dbb16befd5aa82b9149d37c6577450d173d66fb0b638d8377822407d4`  
		Last Modified: Thu, 01 Apr 2021 04:43:07 GMT  
		Size: 1.4 MB (1439817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafae2eed22e4f4b7c690e28391ddf1a273067a5b12e3c4f32827774dd5bdc15`  
		Last Modified: Thu, 01 Apr 2021 04:43:05 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db45b483048b084820a30ce08c132efa2cbc029b60de461a4e5b5e897e48299f`  
		Last Modified: Thu, 01 Apr 2021 04:43:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd522b756a34a4f23f5e58aa3a7fb058e647327976d78979811b8690cb52aa3d`  
		Last Modified: Thu, 01 Apr 2021 04:47:04 GMT  
		Size: 10.4 MB (10353540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e33ac93c2e74a9305906df1452e23ccbdedd01b434bf971eb656ebba4a900e`  
		Last Modified: Thu, 01 Apr 2021 04:47:01 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d09892df0ea0526d8eb917de89f0792a51f9cdbc3a12cc7e963502829ff3ff7`  
		Last Modified: Thu, 01 Apr 2021 04:47:05 GMT  
		Size: 14.7 MB (14659820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297583fe2f221442c4c57897a419a9c85b6c341b9e0bf04d7be94506a63c3f6`  
		Last Modified: Thu, 01 Apr 2021 04:47:01 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229bbbd1ee17cd6dd3814139f1c5f98af229bbdfc7be7b0c046be42efa57f19f`  
		Last Modified: Thu, 01 Apr 2021 04:47:01 GMT  
		Size: 16.9 KB (16877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a671707bff31e85da3249e0c18b47ee85dfaeaee71844f904a0dfb7c1c013c2`  
		Last Modified: Thu, 01 Apr 2021 04:47:01 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8467d5f6b8adf786965cd484fde3c0796b614d0642e7151df359cff44681ac`  
		Last Modified: Thu, 01 Apr 2021 09:34:51 GMT  
		Size: 3.1 MB (3056960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be10fb2b6ba04e7134a07b8dfe1a17291d638d40cefcf0e8e1f28861ce326eda`  
		Last Modified: Thu, 01 Apr 2021 09:34:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f9ac687364c5f2548b2d991b796a573ea67bf9176eba175f267721fb2f2812`  
		Last Modified: Thu, 01 Apr 2021 19:15:54 GMT  
		Size: 553.0 KB (553008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354f85128657ca6501e5095dc5989cb609620c3fe3b8670fd667a6cddac72451`  
		Last Modified: Thu, 01 Apr 2021 19:15:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb8a425112f1742076a9994f6495c48dccdb3cdf0bed3d57bb783d2cb57b29f`  
		Last Modified: Thu, 01 Apr 2021 19:15:58 GMT  
		Size: 18.8 MB (18827390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; ppc64le

```console
$ docker pull drupal@sha256:a52217d55b4954c923292301140aa873ffdd8165e84be9b3dee8d2d60dca2962
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52264918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9facd22f44b0d63a9c86d5f46287580c0c006ea81453f48c579083911d97be98`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 22:04:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 22:05:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 22:05:25 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 22:05:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 22:05:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 22:11:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 22:11:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 22:12:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 22:12:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 22:47:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 22:47:28 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 22:47:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 22:47:46 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 22:48:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 22:48:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 22:52:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 22:52:28 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 22:53:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 22:53:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 22:53:39 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 22:54:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 22:54:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 22:54:13 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 22:54:21 GMT
CMD ["php-fpm"]
# Fri, 02 Apr 2021 05:20:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Apr 2021 05:20:28 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Apr 2021 05:20:30 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Fri, 02 Apr 2021 05:20:34 GMT
ENV DRUPAL_VERSION=9.1.5
# Fri, 02 Apr 2021 05:20:37 GMT
WORKDIR /opt/drupal
# Fri, 02 Apr 2021 05:21:02 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 02 Apr 2021 05:21:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9419926485e714786eb20b7eb5cddc3574a440af1413622feea82302dd7d50eb`  
		Last Modified: Thu, 01 Apr 2021 23:47:54 GMT  
		Size: 1.4 MB (1383186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f862a619e55f20cb796df3edd9f18562b5ddf486d1b216aae0b99287bef1a9`  
		Last Modified: Thu, 01 Apr 2021 23:47:53 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cd54117ef328fe730dd1cb898fb4c4d348136267dc726c3595c65d680f06ff`  
		Last Modified: Thu, 01 Apr 2021 23:47:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5f27598636dcfc16e32b2a0596a0333abe67b41ecbec08a75525ac91ffa70d`  
		Last Modified: Thu, 01 Apr 2021 23:50:56 GMT  
		Size: 10.4 MB (10353562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412e449ebcb27bccf7c44a5670125bebd05b7e873f2d2f14fb7f781690bda958`  
		Last Modified: Thu, 01 Apr 2021 23:50:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217d239ad37ca83d2e745bec17534f63da878a0c9eea7630ea846ba4db41b026`  
		Last Modified: Thu, 01 Apr 2021 23:50:54 GMT  
		Size: 15.3 MB (15259809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289565fe532f9d07a68a28697cf1b7e2a55a921e6f5cf9ca7551833fe3b38a09`  
		Last Modified: Thu, 01 Apr 2021 23:50:50 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290b4de13d3428522ceba73333ea3e70b95101768855bedd1b1e2e4af4834ce7`  
		Last Modified: Thu, 01 Apr 2021 23:50:50 GMT  
		Size: 16.9 KB (16930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04935a2a6a15e3f2a0f89aea4e5cc6967056aa61233cb8f85b4ea4a02e33ab32`  
		Last Modified: Thu, 01 Apr 2021 23:50:50 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ddce426fdd459c79ac9bf9b8ffede5d08401a0b97f4dfa17d0c38947ca74b3`  
		Last Modified: Fri, 02 Apr 2021 05:50:06 GMT  
		Size: 3.1 MB (3051947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea438a9add070138635db77eb1e5c61a5bb251112c4c62bf7f73dc797b605eef`  
		Last Modified: Fri, 02 Apr 2021 05:50:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35e6a4243ac264f2bcbd6d0dcb0f368c641a036c45dfda2fb84b68135c23cdc`  
		Last Modified: Fri, 02 Apr 2021 05:50:04 GMT  
		Size: 553.0 KB (553001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50303ed480e778822bb3fcf724df96d61d89466fade46a999cb573e07e7c24e`  
		Last Modified: Fri, 02 Apr 2021 05:50:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9855b474b6c1e53c43d728ecf177a26dfa90e723e3c847a0a95ea41a9bfb2`  
		Last Modified: Fri, 02 Apr 2021 05:52:32 GMT  
		Size: 18.8 MB (18827205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; s390x

```console
$ docker pull drupal@sha256:5c4780327ca1228da4a441ebefa06cd10663031b01e5dc88d770b6aeca306503
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50192142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c066ca6068906782c6dae6ba05a2636a848f20236e9dd4ae89ba974966240af`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:20:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 01:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 01:20:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 01:20:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 01:20:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 01:42:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 01:42:23 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 01:42:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 01:42:24 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 01:42:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:42:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:45:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:45:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:45:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:45:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:45:48 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 01:45:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 01:45:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 01:45:50 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 01:45:51 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 04:44:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 04:44:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:03:04 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:03:05 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:03:06 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:03:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:03:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f75ff5798a3be1bbf9691a3973afbe2cac00ea8c1f975b8b60d0b93b0b0e84`  
		Last Modified: Thu, 01 Apr 2021 02:25:58 GMT  
		Size: 1.4 MB (1382756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ffde9ee48b9893e4b0d2bd8df2b125908e31b9101fe101724f1123a8d1ff04`  
		Last Modified: Thu, 01 Apr 2021 02:25:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9afdc302e5e2c38c9828e1a1732a2b7d051d2a78bf81eace5124f0630ee38a`  
		Last Modified: Thu, 01 Apr 2021 02:25:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06f783703f08e02ac72c8e6c2f2853ae5cfe9bfc68f3125232cb02ff0df19bd`  
		Last Modified: Thu, 01 Apr 2021 02:28:24 GMT  
		Size: 10.4 MB (10353550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8412f453ba7198910302b5ce729999120b62bc933f2996f2e167b0657927c0d`  
		Last Modified: Thu, 01 Apr 2021 02:28:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b0c2785b8a2e746cef1b366815672b2893efe05bb90b5a03fe5fd59c553828`  
		Last Modified: Thu, 01 Apr 2021 02:28:27 GMT  
		Size: 13.6 MB (13572466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77278072687fe8e0df354fa542a8fd8d3ad633c5bff7d5c39809329c9350bcab`  
		Last Modified: Thu, 01 Apr 2021 02:28:25 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52858dc2c9a68563e26a956aa3283f5502c0adcff39bd2560ff5a2457a0a4c98`  
		Last Modified: Thu, 01 Apr 2021 02:28:22 GMT  
		Size: 16.9 KB (16883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78b17085b3060f962cf4f13508d0bfe983c47804162409c733c6419c254618a`  
		Last Modified: Thu, 01 Apr 2021 02:28:21 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5315cc35503ad71203fec92c6d39143a6745b3102993559ee325d734123d478b`  
		Last Modified: Thu, 01 Apr 2021 04:49:26 GMT  
		Size: 2.9 MB (2905504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f465540ecba1bae5f2712ad1a9249939480fa183fd81767ad9d1119416b33`  
		Last Modified: Thu, 01 Apr 2021 04:49:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e791531aec5bf9754a331378e7fffe605fa86836ef82add685a58109666162ae`  
		Last Modified: Thu, 01 Apr 2021 19:19:42 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a893ee01de61a49aa44032e3cad993679257966dbad2e666ed2f295e45fd3774`  
		Last Modified: Thu, 01 Apr 2021 19:19:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9f0bc3fe344bac6d6c845f399d971c6239975853ea6c9865647c2652f618a8`  
		Last Modified: Thu, 01 Apr 2021 19:19:50 GMT  
		Size: 18.8 MB (18827308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
