## `drupal:php8.0-fpm-alpine3.12`

```console
$ docker pull drupal@sha256:1daf8caf3171555ddd531b574418b2be4d147a76be496cf96025df02e6c137f3
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

### `drupal:php8.0-fpm-alpine3.12` - linux; amd64

```console
$ docker pull drupal@sha256:952bb10922c1093465599bf7e866ef82702d991fc1ef38bd320b923ce0a5e0de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52387605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b275d64e3664b03ad6756bc81e26584c7fc9244286c6b3402f469667f88059fe`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:11:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Feb 2021 00:11:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Feb 2021 00:11:05 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Feb 2021 00:11:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Feb 2021 00:11:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Feb 2021 00:21:12 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 25 Feb 2021 00:21:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 00:21:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 00:21:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 25 Feb 2021 00:21:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Feb 2021 00:21:14 GMT
ENV PHP_VERSION=8.0.2
# Thu, 25 Feb 2021 00:21:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Thu, 25 Feb 2021 00:21:14 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Thu, 25 Feb 2021 00:21:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 00:21:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:31:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 00:31:10 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:31:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 00:31:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 00:31:13 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 00:31:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 00:31:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 00:31:16 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 00:31:16 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 04:23:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 04:23:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 04:23:43 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:23:43 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 04:23:43 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 04:23:52 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 04:23:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad74aaae8c203add54cdf98e07d2dbb763e180a60f960c37d088d9eb13071a`  
		Last Modified: Thu, 25 Feb 2021 01:25:15 GMT  
		Size: 1.3 MB (1340838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b226acec8aca091881202e86b06ba7ec06b97b0086fe639cb063f99e8c7a974`  
		Last Modified: Thu, 25 Feb 2021 01:25:15 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bf1f940f0c78db7a75454ec51fcb5c81e01d550ef1ca775e19ee1ee03ae112`  
		Last Modified: Thu, 25 Feb 2021 01:25:15 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd89103d06bcd9c668be582d6a92bd6f671a4f20f662fcff58e3fe090cc7471f`  
		Last Modified: Thu, 25 Feb 2021 01:25:33 GMT  
		Size: 10.7 MB (10669367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4e889aca73989427b88d3740b255beab882921498b50b96899bfa56bcd111b`  
		Last Modified: Thu, 25 Feb 2021 01:25:31 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d6a5cd428c3ee78e7248318244b49cea30def2a5bd6e4f82719c2749cedbcc`  
		Last Modified: Thu, 25 Feb 2021 01:25:34 GMT  
		Size: 15.0 MB (14965027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e72861b7a189bdf1f5b9e3511438d00d75eb207bd58b0882e00a3e10249d18`  
		Last Modified: Thu, 25 Feb 2021 01:25:31 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07157556b5c4693859e8c5da7828649dd6ae1bb1d7cb35aef4c48ffdd774d596`  
		Last Modified: Thu, 25 Feb 2021 01:25:31 GMT  
		Size: 16.9 KB (16894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531c05c9a4fa65099ff73cd67723e73cd73e96e6532a11763934c5629b7d3f5`  
		Last Modified: Thu, 25 Feb 2021 01:25:31 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38afbf5bdb8e066dde9d04923a9939ea6ae876bc3e3b284cad7711ccfebdd57a`  
		Last Modified: Thu, 25 Feb 2021 04:29:04 GMT  
		Size: 3.2 MB (3211599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfe1177b92f60bf898078e7ccb9c766ae7e244d7ee3c8fcefaf2ab760600606`  
		Last Modified: Thu, 25 Feb 2021 04:29:03 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f8e0d4fcde5ebcd1574cd168fafd77a8581841d77b5e37fa01ba23c374451`  
		Last Modified: Thu, 25 Feb 2021 04:29:03 GMT  
		Size: 551.8 KB (551789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e423f59460e75741a19d08306060507f2a7e9ffde526f4bb1553ef8b935be1`  
		Last Modified: Thu, 25 Feb 2021 04:29:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3316677f1d8914cb60320337f09f70c5f00f3b62c43bb66765e1f3fbd0aedd2`  
		Last Modified: Thu, 25 Feb 2021 04:29:09 GMT  
		Size: 18.8 MB (18819373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; arm variant v6

```console
$ docker pull drupal@sha256:51077b7e2e33ff474b8973abe7ce4b5571bd21bdc3681cb7984ddf567b24631e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50381222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9de7a55e4215dff9e9f11c0986f40a4049aff2de5117eaabeb5179339eb33f48`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:48:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 24 Feb 2021 21:48:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 24 Feb 2021 21:48:51 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 24 Feb 2021 21:48:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 24 Feb 2021 21:48:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 24 Feb 2021 21:53:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 24 Feb 2021 21:53:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 24 Feb 2021 21:53:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 24 Feb 2021 21:53:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 24 Feb 2021 21:53:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 24 Feb 2021 21:53:13 GMT
ENV PHP_VERSION=8.0.2
# Wed, 24 Feb 2021 21:53:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Wed, 24 Feb 2021 21:53:15 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Wed, 24 Feb 2021 21:53:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 24 Feb 2021 21:53:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 24 Feb 2021 21:57:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 24 Feb 2021 21:57:11 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 24 Feb 2021 21:57:14 GMT
RUN docker-php-ext-enable sodium
# Wed, 24 Feb 2021 21:57:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 24 Feb 2021 21:57:18 GMT
WORKDIR /var/www/html
# Wed, 24 Feb 2021 21:57:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 24 Feb 2021 21:57:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 24 Feb 2021 21:57:26 GMT
EXPOSE 9000
# Wed, 24 Feb 2021 21:57:27 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 03:25:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 03:25:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 26 Feb 2021 02:05:51 GMT
COPY file:deb590b59fc201c558f5c400490c99455a4f02093f44f8b429b21b024fa29bb3 in /usr/local/bin/ 
# Fri, 26 Feb 2021 02:05:54 GMT
ENV DRUPAL_VERSION=9.1.4
# Fri, 26 Feb 2021 02:05:55 GMT
WORKDIR /opt/drupal
# Fri, 26 Feb 2021 02:06:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 26 Feb 2021 02:06:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615a3cb7c8a689c7b4b457673e4a5678045e9719205698379bb794653438a8f8`  
		Last Modified: Wed, 24 Feb 2021 22:25:14 GMT  
		Size: 1.3 MB (1310252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779c61c3f721398235ceaccb55a3fb089907ab61a3bc41f3fe457c740545a965`  
		Last Modified: Wed, 24 Feb 2021 22:25:14 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f577d474ce74b9771d890356acf5aab30aa563d9c7c2edf98725de2e1c194d4`  
		Last Modified: Wed, 24 Feb 2021 22:25:13 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e66145507f6266ac5f8efc897c318e0f9ed906f0c6486d89d8d0d9d8f1b069`  
		Last Modified: Wed, 24 Feb 2021 22:25:34 GMT  
		Size: 10.7 MB (10669392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492db1a779cc206904aa917317a87bb4b2d945cc25dc00e9ccbd8f46fb7c125d`  
		Last Modified: Wed, 24 Feb 2021 22:25:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87010d6976a59aba3620f0dd9e1721db916ea698b7c271a4c30af62413ca3e19`  
		Last Modified: Wed, 24 Feb 2021 22:25:36 GMT  
		Size: 13.6 MB (13646606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87a8505a06af70bf2563e57e07dbd2b3c7a94f412c49e8c49f4369836193e5b`  
		Last Modified: Wed, 24 Feb 2021 22:25:31 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3574b2f0fdb923932d82ecc5069b70866d4c93211e64261aeb82923526e19f4`  
		Last Modified: Wed, 24 Feb 2021 22:25:31 GMT  
		Size: 16.9 KB (16888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97322029cb953812be968242b03004e00c90c4f993d473cbabe44f2c7f13104`  
		Last Modified: Wed, 24 Feb 2021 22:25:31 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383f24c463ccb8f26bc527e96fb25e1cb28cf1fe999f9849d1da79083dc3e592`  
		Last Modified: Thu, 25 Feb 2021 03:30:48 GMT  
		Size: 2.7 MB (2748665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602be0be6c4bf922efbf86131dc96e6da7f00a5f4625086b020aee1aaca3291c`  
		Last Modified: Thu, 25 Feb 2021 03:30:47 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bb06e42eb433bfbbb4eb3288b5e76fc2db29a862f1a4696e71f2f02098b3cd`  
		Last Modified: Fri, 26 Feb 2021 02:08:16 GMT  
		Size: 551.8 KB (551807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a56c07f893f4b81fb7afbdba924ddff31dc3ab3a2d09017b340ea64268b593`  
		Last Modified: Fri, 26 Feb 2021 02:08:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4479b141079562ceb0efc3bfa7b30596468a1914c73ee172305bed00aabb3cd0`  
		Last Modified: Fri, 26 Feb 2021 02:08:27 GMT  
		Size: 18.8 MB (18819758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0cb9b25d801f970d4e849b8679d736a37bb21e1849ab5e71f8db799c94254dbe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48974651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9148e90a26ee61a7c3df7225e3c85adc3b5579b3569e715d1e5aa81b8e184e1b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:38:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Feb 2021 00:38:52 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Feb 2021 00:39:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Feb 2021 00:39:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Feb 2021 00:39:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Feb 2021 00:45:45 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 25 Feb 2021 00:45:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 00:45:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 00:45:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 25 Feb 2021 00:45:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Feb 2021 00:45:53 GMT
ENV PHP_VERSION=8.0.2
# Thu, 25 Feb 2021 00:45:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Thu, 25 Feb 2021 00:45:54 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Thu, 25 Feb 2021 00:46:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 00:46:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:49:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 00:49:16 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:49:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 00:49:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 00:49:27 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 00:49:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 00:49:35 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 00:49:37 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 00:49:38 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 03:04:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 03:04:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 03:04:08 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 03:04:09 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 03:04:10 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 03:04:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 03:04:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14cc8b4ab32066557eac8444fa33ee5ebaed36826b316cd88df2b9cb3005d89`  
		Last Modified: Thu, 25 Feb 2021 01:29:39 GMT  
		Size: 1.2 MB (1214324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3820ceb6aa3721ffa3c4431d838261590e757f46b57b8598c1ec5ec4262a2a4`  
		Last Modified: Thu, 25 Feb 2021 01:29:38 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e3ecf788cb43363fdced38ca2f1e332603abf470c39ac131d849811ca5e95`  
		Last Modified: Thu, 25 Feb 2021 01:29:38 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b142c29fb7b55970e94dcef4cf631267990c682944193d69f79e7b33048f0b`  
		Last Modified: Thu, 25 Feb 2021 01:30:12 GMT  
		Size: 10.7 MB (10669384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36dfba21e4c07a3bc76816797b0ff63a334acff04c4167fb87c66929d9d869c`  
		Last Modified: Thu, 25 Feb 2021 01:30:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f23760022d9c53196002bfb7e32efdf906fe036c8dd3bec3aad8de97fab59`  
		Last Modified: Thu, 25 Feb 2021 01:30:15 GMT  
		Size: 12.8 MB (12788157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb4ffbc82e092b3a3cace964c2261f3418f9ee3f6d86dfb14ba758a459cbfef`  
		Last Modified: Thu, 25 Feb 2021 01:30:08 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebadbdce53bb960ddaeeb2cc368e1bbad5832e754737e4db0a122b0fe1f48e8`  
		Last Modified: Thu, 25 Feb 2021 01:30:07 GMT  
		Size: 16.9 KB (16865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a3a80a690e2cbb0fd2361dc776c0acb55c338469508fe113354a020fc909f9`  
		Last Modified: Thu, 25 Feb 2021 01:30:07 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5b911290672732942df6b8986d24dd00a049ca93923e5cf675b31fa2d028a9`  
		Last Modified: Thu, 25 Feb 2021 03:12:04 GMT  
		Size: 2.5 MB (2493213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54090e719ab61bef3e4abfbb772064923765e2ee0226ee6a587aef7a97dd1439`  
		Last Modified: Thu, 25 Feb 2021 03:12:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584b52c91f70d974cd59d9cf143113dfbce2ef3001cb9694ea3571557e1670b2`  
		Last Modified: Thu, 25 Feb 2021 03:12:04 GMT  
		Size: 551.8 KB (551792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73a945ac9644d9593c86ceb4879c5c11f531129e1181d3387db747512fec241`  
		Last Modified: Thu, 25 Feb 2021 03:12:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7464293c4755e8dc5439befc97e5d7d6dae7eb205ff3b35bb639a3fad4072fce`  
		Last Modified: Thu, 25 Feb 2021 03:12:18 GMT  
		Size: 18.8 MB (18819567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:b5555e79951dfb1a3066dbd9ef6efa53978027617b8bad159f8081e98db61045
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51447249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a55243dbe7767f9e3348b721e682b7cca67668c52a2d18e13a28520d61b0a0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:15:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Feb 2021 02:15:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Feb 2021 02:15:24 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Feb 2021 02:15:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Feb 2021 02:15:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Feb 2021 02:19:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 25 Feb 2021 02:19:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 02:19:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 02:19:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 25 Feb 2021 02:19:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Feb 2021 02:19:53 GMT
ENV PHP_VERSION=8.0.2
# Thu, 25 Feb 2021 02:19:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Thu, 25 Feb 2021 02:19:55 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Thu, 25 Feb 2021 02:20:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 02:20:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:24:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 02:24:07 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:24:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 02:24:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 02:24:15 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 02:24:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 02:24:21 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 02:24:22 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 02:24:23 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 05:30:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 05:30:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 05:30:12 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 05:30:12 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 05:30:13 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 05:30:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 05:30:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd265321b6926cee038cf7fc6338237aac197c6c9ef85b1982906eb78e6ea2c`  
		Last Modified: Thu, 25 Feb 2021 02:52:50 GMT  
		Size: 1.3 MB (1342954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb80a7dbf57a115e70afd93274767256a51782fee74606762ff0c3bbbd5b91d1`  
		Last Modified: Thu, 25 Feb 2021 02:52:50 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba32dc0c8f3fa39e73379ea7a837a9987f419051e77502e949be24d45d001ae2`  
		Last Modified: Thu, 25 Feb 2021 02:52:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2fead4195200ef55f77630a84cb438ba7618f60e4c9f1b7687785829505a0d`  
		Last Modified: Thu, 25 Feb 2021 02:53:09 GMT  
		Size: 10.7 MB (10669388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfb4b0e4488e82c51df04a2a71524646594b8dcd7e1473862f21b635e02e3a1`  
		Last Modified: Thu, 25 Feb 2021 02:53:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd315e48bd8fa8c4a964b586b11d62e7ed51b105595180f736a0e4945157a3f`  
		Last Modified: Thu, 25 Feb 2021 02:53:11 GMT  
		Size: 14.4 MB (14433776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf431e673cd17c861553988edbd7b2c6e0809d1cc85849827bbf9318776ba6d`  
		Last Modified: Thu, 25 Feb 2021 02:53:07 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f334fbad6d417b4b1d04c4fae969bc1615d206939bd68dc8ffd0ce6eede9c08a`  
		Last Modified: Thu, 25 Feb 2021 02:53:08 GMT  
		Size: 16.9 KB (16897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960ebf9415682da582e870dc2d1346a91a45d37ea8fe1555f13b9a9a3be97e37`  
		Last Modified: Thu, 25 Feb 2021 02:53:07 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb88dff0df4da9fad8d5bde2d546da49a85d6ef2c173835cd61aa281d29c3eb`  
		Last Modified: Thu, 25 Feb 2021 05:38:11 GMT  
		Size: 2.9 MB (2889281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43f3649bc7e45d14c7b859da7d673c276599bf09b3ce04f3bbcfdf16bda2c43`  
		Last Modified: Thu, 25 Feb 2021 05:38:11 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2721a02cbcf3d3642792d0b0fc62b02c28e4b1cc121f2961c237a5f8b3b70`  
		Last Modified: Thu, 25 Feb 2021 05:38:10 GMT  
		Size: 551.8 KB (551785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142aecf3032224c03d2469bfef0d755acf50773e92708be615e0b925cfe005c9`  
		Last Modified: Thu, 25 Feb 2021 05:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a540dfff2b5b4e331fa48eb21db6a8a5790b69062c17114f5d8a4b5acb8e8640`  
		Last Modified: Thu, 25 Feb 2021 05:38:18 GMT  
		Size: 18.8 MB (18819955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; 386

```console
$ docker pull drupal@sha256:c0b5030405de00bbd043b226b4de4846c17d1d8cf74f6c38c09af75dbcbe04cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52391613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8eec6ecd6d8cedbcbadf55a25b0494f29a40008bace770e2d00bab5d707ead4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:32:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 24 Feb 2021 23:32:41 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 24 Feb 2021 23:32:42 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 24 Feb 2021 23:32:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 24 Feb 2021 23:32:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 24 Feb 2021 23:40:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 24 Feb 2021 23:40:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 24 Feb 2021 23:40:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 24 Feb 2021 23:40:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 24 Feb 2021 23:40:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 24 Feb 2021 23:40:18 GMT
ENV PHP_VERSION=8.0.2
# Wed, 24 Feb 2021 23:40:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Wed, 24 Feb 2021 23:40:18 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Wed, 24 Feb 2021 23:40:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 24 Feb 2021 23:40:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 24 Feb 2021 23:47:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 24 Feb 2021 23:47:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 24 Feb 2021 23:47:04 GMT
RUN docker-php-ext-enable sodium
# Wed, 24 Feb 2021 23:47:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 24 Feb 2021 23:47:04 GMT
WORKDIR /var/www/html
# Wed, 24 Feb 2021 23:47:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 24 Feb 2021 23:47:05 GMT
STOPSIGNAL SIGQUIT
# Wed, 24 Feb 2021 23:47:05 GMT
EXPOSE 9000
# Wed, 24 Feb 2021 23:47:06 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 02:37:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 02:37:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 02:37:24 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:37:24 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 02:37:24 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 02:37:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 02:37:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fa6c39d261a8412d9912cec351f6b689cbe9b9d3e83f4e6c853980e909db2d`  
		Last Modified: Thu, 25 Feb 2021 00:42:48 GMT  
		Size: 1.4 MB (1439676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a3072d60564d935173bb27f3635efd9016798160e53980cd17becdb7ff2770`  
		Last Modified: Thu, 25 Feb 2021 00:42:46 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4363a86ea77cb1ad1e167f8823b603160ccbb145adf775327a6fc9609b8a0855`  
		Last Modified: Thu, 25 Feb 2021 00:42:46 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b115519f4c1429b413774f30d31545f3196cd0edd33e0d9e8128e7cb8d0f75`  
		Last Modified: Thu, 25 Feb 2021 00:43:14 GMT  
		Size: 10.7 MB (10669344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3c46280f2d35277c7487e3553b7c3c995691db7b495839366e2a36b6413dfa`  
		Last Modified: Thu, 25 Feb 2021 00:43:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8a9ebcf3f8208bf10570d9b29b413f91db610db83bc0e17c387496e75d6591`  
		Last Modified: Thu, 25 Feb 2021 00:43:20 GMT  
		Size: 15.0 MB (15008168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4af997a0afe5b98526ff97880a8df958f130625335ad42a8bed02a834da9454`  
		Last Modified: Thu, 25 Feb 2021 00:43:10 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21f11cfb7eebbc754f2b91e0c422a72514c8d2615f8701944f1b5734634420d`  
		Last Modified: Thu, 25 Feb 2021 00:43:10 GMT  
		Size: 16.9 KB (16874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52948b33a92cd98347da7f29aaca5ffd11cc0179ee147cdb0fb57ce89b497672`  
		Last Modified: Thu, 25 Feb 2021 00:43:11 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a52b3c0833869ef64e1e0244d3251e1fa1f94703a4ca98ecf32cd88acbaeea1`  
		Last Modified: Thu, 25 Feb 2021 02:45:12 GMT  
		Size: 3.1 MB (3078058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab2717abb7aeb0001cd678186c30ea3990fc7f0f4aa48e4ff04a0324d794a8e`  
		Last Modified: Thu, 25 Feb 2021 02:45:07 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2583805235f464c69db8b66dd58e52989c43f59d680a3bb043a097c198ed2466`  
		Last Modified: Thu, 25 Feb 2021 02:45:08 GMT  
		Size: 551.8 KB (551787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c02336252bee80c58757708e05e5f255706ff20afc722c5a8c1cf53bbab2645`  
		Last Modified: Thu, 25 Feb 2021 02:45:07 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab618a687e58f84c744a8ac8eba2b4052109680f44824486d115a8ca9036147`  
		Last Modified: Thu, 25 Feb 2021 02:45:18 GMT  
		Size: 18.8 MB (18819745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; ppc64le

```console
$ docker pull drupal@sha256:b6d1d043ca34dca2e9c2b39705827c2d582f9ef20b6c6a60cc8afc1b70e25c02
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52978298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d683c16321f3fcaff548c03a04df979582adc63a15054fb9d7264aece0e1363`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:45:10 GMT
ADD file:90df4b3d767cd67ff62e490ca0a7d69bae532cf3fa6f8971a0d2c1b27fb4bdd1 in / 
# Wed, 24 Feb 2021 20:45:16 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:18:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Feb 2021 02:18:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Feb 2021 02:19:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Feb 2021 02:19:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Feb 2021 02:19:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Feb 2021 02:25:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 25 Feb 2021 02:25:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 02:25:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 02:25:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 25 Feb 2021 02:25:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Feb 2021 02:25:56 GMT
ENV PHP_VERSION=8.0.2
# Thu, 25 Feb 2021 02:26:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Thu, 25 Feb 2021 02:26:05 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Thu, 25 Feb 2021 02:26:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 02:26:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:30:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 02:30:39 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:31:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 02:31:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 02:31:19 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 02:31:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 02:31:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 02:31:41 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 02:31:54 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 05:09:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 05:09:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 05:09:17 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 05:09:22 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 05:09:31 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 05:10:04 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 05:10:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8f446c8f22d4a7a7520099080f73ffa6f455358a840b542fb2ad15c0032adeca`  
		Last Modified: Wed, 24 Feb 2021 20:46:19 GMT  
		Size: 2.8 MB (2805893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442844d8617592bb8b8a6a6806933d8ce610ddeb989712f03f8abc7daf0e8a09`  
		Last Modified: Thu, 25 Feb 2021 03:09:38 GMT  
		Size: 1.4 MB (1383188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765d755a8614ffa2086b17c3a59d50abbd5a7f85bf41d5c5424d6b7ac1d9aeff`  
		Last Modified: Thu, 25 Feb 2021 03:09:37 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec8dadfb9e7f832d4e8acd90c13b1450c86379a9bc45045f7fca480e61ce4a6`  
		Last Modified: Thu, 25 Feb 2021 03:09:37 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069559f7b2531a483401027eb967f726a2ab1ff4ef3c3a5cd1a054f504e52518`  
		Last Modified: Thu, 25 Feb 2021 03:10:10 GMT  
		Size: 10.7 MB (10669392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123e3d463144d278dab79311035675589f4a4c2785989b116d20bf2a4883a796`  
		Last Modified: Thu, 25 Feb 2021 03:10:05 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3f90953d569cff92db55bd77c565474982f25348c54ea8e145dc60d4ca1d1e`  
		Last Modified: Thu, 25 Feb 2021 03:10:09 GMT  
		Size: 15.6 MB (15647266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fc3ac48bcd8edcf408cddfedbb25dfd955c46dc564919247368a82aeb3d27a`  
		Last Modified: Thu, 25 Feb 2021 03:10:06 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564bf7bd97f4ec3959faa035e2127dd0f7d4ee9b99197f2d72e58068eb3ca32a`  
		Last Modified: Thu, 25 Feb 2021 03:10:06 GMT  
		Size: 16.9 KB (16928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c503ba3c170eae64e556abea007f39116270ffeb7dc3e6530e803b1604e0b9`  
		Last Modified: Thu, 25 Feb 2021 03:10:06 GMT  
		Size: 8.6 KB (8575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b531af8b3618c80ad1dabeb901ad4700f6fdfeb8a45732b50b99fa9e00fbf63`  
		Last Modified: Thu, 25 Feb 2021 05:22:27 GMT  
		Size: 3.1 MB (3070811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c474f6b9681881ddc9dd67532c97ddaa4219fde49dcdc54ea7b487c5e16350c`  
		Last Modified: Thu, 25 Feb 2021 05:22:27 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c13027c50f48c2a3c324a9180a9520b333bab893d1310b149f2ea11f610f9`  
		Last Modified: Thu, 25 Feb 2021 05:22:26 GMT  
		Size: 551.8 KB (551789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed28fc0834cd7bcf2889afb20a747f502c5009b6b819968e8c5e380f4b23aab`  
		Last Modified: Thu, 25 Feb 2021 05:22:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e493b20adf04733ec10af9d3d068abe409279c260e3b90c59827f160576d0e`  
		Last Modified: Thu, 25 Feb 2021 05:22:32 GMT  
		Size: 18.8 MB (18819688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.12` - linux; s390x

```console
$ docker pull drupal@sha256:337c1d16adaf2085ac14d48b5f85c0f98e5019542bd3e2c00544ef72a6986d30
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50872052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c784dc161521dbb181f3b8bbda07574c112e58ad16b2eefc3eaa5e24c0de191a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Feb 2021 20:42:00 GMT
ADD file:ad5b3d24d5412d341e932d4497614d564c9c413984feaf8542113d6674b34b53 in / 
# Wed, 24 Feb 2021 20:42:01 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:59:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Feb 2021 03:59:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Feb 2021 03:59:24 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Feb 2021 03:59:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Feb 2021 03:59:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Feb 2021 04:07:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 25 Feb 2021 04:07:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 04:07:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Feb 2021 04:07:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 25 Feb 2021 04:07:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Feb 2021 04:07:08 GMT
ENV PHP_VERSION=8.0.2
# Thu, 25 Feb 2021 04:07:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Thu, 25 Feb 2021 04:07:10 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Thu, 25 Feb 2021 04:07:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 04:07:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:13:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 04:13:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:13:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 04:13:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 04:13:53 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 04:13:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 04:13:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 04:13:56 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 04:13:56 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 06:39:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 06:39:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 06:39:56 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 06:39:57 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 06:39:58 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 06:40:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 06:40:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:84a604a54099b51a6c81db20dff8dc298ec82555e772be84328b067d3f35a93e`  
		Last Modified: Wed, 24 Feb 2021 20:42:40 GMT  
		Size: 2.6 MB (2567318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c953dc38bcd2ea5c92ba4d4476c130d7fd6f9f7578a631aef0adba4853dafe7`  
		Last Modified: Thu, 25 Feb 2021 04:54:13 GMT  
		Size: 1.4 MB (1382770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f039ee07371753cd0e27c5060a8a15f3ea3b8e8a72ad3810d5cd6275421432f`  
		Last Modified: Thu, 25 Feb 2021 04:54:14 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417921f8bb3225d1c8e8390bff5eb08298a9ac6e24b211a4fccd11659f56625b`  
		Last Modified: Thu, 25 Feb 2021 04:54:12 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce5083cc29c34098ffaa4cc0fd492816916d26fd1f57a0ef2946fa40c679257`  
		Last Modified: Thu, 25 Feb 2021 04:54:35 GMT  
		Size: 10.7 MB (10669389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299dfbaca54af0c927096320bd3313b9b017bedc27c69b87056978b87123660`  
		Last Modified: Thu, 25 Feb 2021 04:54:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c2f1c4f93a9226e01a8ffceb93946b0bbe91cf0ca6c5256309253cb880b1cf`  
		Last Modified: Thu, 25 Feb 2021 04:54:35 GMT  
		Size: 13.9 MB (13931308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7846245177530541ab0687bcf03ad902fe3334683eb7c739e53c79eabb39b65`  
		Last Modified: Thu, 25 Feb 2021 04:54:33 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ba9501296e3194c62757a1b46dc2741f6fa6d157776ca54bd9fc8d430e11a7`  
		Last Modified: Thu, 25 Feb 2021 04:54:33 GMT  
		Size: 16.9 KB (16886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06179c006b3f3bf08da8fd078bfdc4b81ecf705032baea8fa7b51a5d0969b8d`  
		Last Modified: Thu, 25 Feb 2021 04:54:33 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcff896a49e78421aec06897250c309a9e848fce6646dcd1a0b159ddfef557b`  
		Last Modified: Thu, 25 Feb 2021 06:48:42 GMT  
		Size: 2.9 MB (2919550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8560ceb90fe545c1a5aa7ed8790fd58feb242db5addb807d4b1af20f84a554`  
		Last Modified: Thu, 25 Feb 2021 06:48:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df356e656f0dc9f8c6700230533c8e760287133f9626ca0719e2652f84e20ae2`  
		Last Modified: Thu, 25 Feb 2021 06:48:41 GMT  
		Size: 551.8 KB (551786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa0a9e5555447d51874a6460e0f4584a7f9036ba7914acfd4f7894f831c6cf7`  
		Last Modified: Thu, 25 Feb 2021 06:48:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b6631e8d491ef70388a432234963462f895a8f45badcb75dc4327ccae72ac6`  
		Last Modified: Thu, 25 Feb 2021 06:48:45 GMT  
		Size: 18.8 MB (18819709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
