## `drupal:php7.4-fpm-alpine3.12`

```console
$ docker pull drupal@sha256:bd8befcd8763fa7f2bef3b716af4931cca0a7218ae7428c73cb426872f167d28
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
$ docker pull drupal@sha256:e488d95f4d9447c806abb276f50438ef67b77053bebde9090b940a1f807a4fa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (51029483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b68c706d2b0ef901d60ea97405dff461d634f62530bacdc80eb4856e3b557a`
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
# Thu, 25 Feb 2021 00:40:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Feb 2021 00:40:28 GMT
ENV PHP_VERSION=7.4.15
# Thu, 25 Feb 2021 00:40:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 25 Feb 2021 00:40:28 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 25 Feb 2021 00:40:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 00:40:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:46:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 00:46:19 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:46:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 00:46:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 00:46:21 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 00:46:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 00:46:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 00:46:23 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 00:46:23 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 04:24:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 04:24:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 04:24:54 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:24:54 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 04:24:54 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 04:25:04 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 04:25:04 GMT
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
	-	`sha256:d191ab097c06b30863174552d4a5a20637c5900da790881cd7889f5ed1a55ef4`  
		Last Modified: Thu, 25 Feb 2021 01:26:18 GMT  
		Size: 10.4 MB (10351195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109c212479b2777c97ce1e10c6750d98f95d9ba14a8ba17db9ecc4daa029537f`  
		Last Modified: Thu, 25 Feb 2021 01:26:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adae70203d21a9f940097e4994af6677986a79451d48a1e85bc791f7674886ce`  
		Last Modified: Thu, 25 Feb 2021 01:26:19 GMT  
		Size: 14.3 MB (14275427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c021bdfe37217d88b494f60d22dab7dbf2081345eef810b5cccd5e817ec02d9`  
		Last Modified: Thu, 25 Feb 2021 01:26:16 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc6fb52e58ed564a6324e879e9cc01827621a8a2f9b9706852296e97e99935c`  
		Last Modified: Thu, 25 Feb 2021 01:26:16 GMT  
		Size: 16.9 KB (16892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0100fc1ac1fe29303f47fca541a119c6619dfaf7c0cd4bd30e16e96e30173b6`  
		Last Modified: Thu, 25 Feb 2021 01:26:16 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0e7f91d0754dfcea5c9634a63b8f46671c673688e0cf831abcbfc7fcb6b725`  
		Last Modified: Thu, 25 Feb 2021 04:29:35 GMT  
		Size: 2.9 MB (2861069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5a4ce2565020978f663b43374759b2b69f0cb4a5b7f647b2f2a913a74dd92`  
		Last Modified: Thu, 25 Feb 2021 04:29:34 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51259850ea0df72ae30d76ddaff0475454df380acd543fc71130cbee3463d161`  
		Last Modified: Thu, 25 Feb 2021 04:29:35 GMT  
		Size: 551.8 KB (551789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae993f55b37bce69800f1854710863b110a7a9f4f7fc4cd190e8f649f31a53e3`  
		Last Modified: Thu, 25 Feb 2021 04:29:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61b4cef3161bfa16ee7bb8a805dd49fcd328111e544c6e53b1cbeb3cf6aedc9`  
		Last Modified: Thu, 25 Feb 2021 04:29:40 GMT  
		Size: 18.8 MB (18819686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm variant v6

```console
$ docker pull drupal@sha256:ca6bd264c439224e637f4b7d1dc0768f224c5744a9b570ab6931219c02ec29b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49683959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5d96c4757339e1f1fac48f9faf3490689d7bbacc4d754b392926421c667af4`
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
# Wed, 24 Feb 2021 22:02:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 24 Feb 2021 22:02:05 GMT
ENV PHP_VERSION=7.4.15
# Wed, 24 Feb 2021 22:02:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Wed, 24 Feb 2021 22:02:07 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Wed, 24 Feb 2021 22:02:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 24 Feb 2021 22:02:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 24 Feb 2021 22:06:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 24 Feb 2021 22:06:06 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 24 Feb 2021 22:06:10 GMT
RUN docker-php-ext-enable sodium
# Wed, 24 Feb 2021 22:06:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 24 Feb 2021 22:06:11 GMT
WORKDIR /var/www/html
# Wed, 24 Feb 2021 22:06:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 24 Feb 2021 22:06:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 24 Feb 2021 22:06:16 GMT
EXPOSE 9000
# Wed, 24 Feb 2021 22:06:18 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 03:27:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 03:27:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 26 Feb 2021 02:06:39 GMT
COPY file:deb590b59fc201c558f5c400490c99455a4f02093f44f8b429b21b024fa29bb3 in /usr/local/bin/ 
# Fri, 26 Feb 2021 02:06:40 GMT
ENV DRUPAL_VERSION=9.1.4
# Fri, 26 Feb 2021 02:06:40 GMT
WORKDIR /opt/drupal
# Fri, 26 Feb 2021 02:07:06 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 26 Feb 2021 02:07:11 GMT
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
	-	`sha256:9ea175bd79c65dfe98851af10124aa100a1c27374cf3ec069efc0f93a6023950`  
		Last Modified: Wed, 24 Feb 2021 22:26:16 GMT  
		Size: 10.4 MB (10351223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afba043391c1656b922d0bc5ff045425381bff28dccc91ead1c5f592d7abac8e`  
		Last Modified: Wed, 24 Feb 2021 22:26:13 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71ebc7e66acac3bb9cf508cc149ecbfb2c14e27c3722ad8b9c639ba8bc3584`  
		Last Modified: Wed, 24 Feb 2021 22:26:18 GMT  
		Size: 13.3 MB (13285747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800162e94489ff18bdde0914716c034ebc7f6d7278a88bf272eafca65c5f8892`  
		Last Modified: Wed, 24 Feb 2021 22:26:13 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d44bf43fa5c5c0574a628bf332312b7a918e7dd6baf3b08898790210afd243d`  
		Last Modified: Wed, 24 Feb 2021 22:26:14 GMT  
		Size: 16.9 KB (16889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32580566a8034328577afebdc62aa8883db3a73a8268ea2e78a4931c7e75657`  
		Last Modified: Wed, 24 Feb 2021 22:26:14 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2b1bef1a0c2bb62cc07e3b7d95f14b3a544b510bc6b2d614712b814e15c260`  
		Last Modified: Thu, 25 Feb 2021 03:31:28 GMT  
		Size: 2.7 MB (2730362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d71f79c0156a2844133749767a00b5da4d48c1871a6ca94df7182e7f30bb02a`  
		Last Modified: Thu, 25 Feb 2021 03:31:27 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbc7057b37abe27d1cff859edab180f88e6093ef404446902436c8579749316`  
		Last Modified: Fri, 26 Feb 2021 02:08:55 GMT  
		Size: 551.8 KB (551813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e6355ae7dbac1b986fcb62de8df34d4ef6ee352afe25336e98deb5fe882062`  
		Last Modified: Fri, 26 Feb 2021 02:08:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234683c11e645fef5f6c4c0e3cd7c257fa743a9a1a24761ca972a30c756c8f7a`  
		Last Modified: Fri, 26 Feb 2021 02:09:09 GMT  
		Size: 18.8 MB (18819946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm variant v7

```console
$ docker pull drupal@sha256:a0c1c442c5e3eebe709bb48d9d2acbc88ec51897832543045f2d0b412eccc406
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48290026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7d889a5b90905c0ce7337ed1087c49bae7ecf638951732733b55bd23e421aaf`
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
# Thu, 25 Feb 2021 00:59:05 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Feb 2021 00:59:06 GMT
ENV PHP_VERSION=7.4.15
# Thu, 25 Feb 2021 00:59:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 25 Feb 2021 00:59:10 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 25 Feb 2021 00:59:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 00:59:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 01:01:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 01:01:55 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 01:01:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 01:02:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 01:02:06 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 01:02:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 01:02:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 01:02:14 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 01:02:16 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 03:06:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 03:06:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 03:06:06 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 03:06:07 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 03:06:08 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 03:06:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 03:06:41 GMT
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
	-	`sha256:2df600206568f069cb2632c4bb3867f446d998db292c8ebf16e38470d462c41f`  
		Last Modified: Thu, 25 Feb 2021 01:31:27 GMT  
		Size: 10.4 MB (10351215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7334f93d7b1a3d483a281df8abae2b1532bb84e08ed54b0962f1da7978fd3a4`  
		Last Modified: Thu, 25 Feb 2021 01:31:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4263df75ab2373763de0e27fee8aab9cd82611d5553b02114d404bd41c360d36`  
		Last Modified: Thu, 25 Feb 2021 01:31:28 GMT  
		Size: 12.4 MB (12437616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2d1c545f4c0533a063a118767c136e9629a2ca6859b1a1d789f75b8bcaeeb1`  
		Last Modified: Thu, 25 Feb 2021 01:31:23 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf01710d0c5f30db630e6ca4dd8b85eb49b930a339e3982cbf9743f36b84cd4b`  
		Last Modified: Thu, 25 Feb 2021 01:31:23 GMT  
		Size: 16.9 KB (16870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93a13aee2aa2103cc7361c25df2b698f6123bed4d974bf54ba60851ea384557`  
		Last Modified: Thu, 25 Feb 2021 01:31:25 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d448f3cc0cd3893db658e3a798cb2a3c812a21a138e1ae0a7760fd7ce5174f`  
		Last Modified: Thu, 25 Feb 2021 03:13:00 GMT  
		Size: 2.5 MB (2477346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2d52708dfab562e345273ad221bff400ea5d61451de34c440d54f6c900d31e`  
		Last Modified: Thu, 25 Feb 2021 03:13:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a77927598a0a68038802135b6ea19826144a316ed6e687cde74b1afc649b5`  
		Last Modified: Thu, 25 Feb 2021 03:13:00 GMT  
		Size: 551.8 KB (551787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ff4d857ce3883b1381df4b34de63822f18749d7a8edd6b71bdcc49336d2d52`  
		Last Modified: Thu, 25 Feb 2021 03:13:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f05f4cc03d6231edd18c544fc2b4777f3964f01af8f8d1cfe40bdc3e852d2bd`  
		Last Modified: Thu, 25 Feb 2021 03:13:13 GMT  
		Size: 18.8 MB (18819653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:abdaf63bc6109d8dc2cacb2f11009c7fcbc9a21002cfa5efe483133f53ec0159
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50754733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:257ce923d579dc33e8bf5189b52f21c8945663107f667565824126441545aee2`
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
# Thu, 25 Feb 2021 02:29:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Feb 2021 02:29:26 GMT
ENV PHP_VERSION=7.4.15
# Thu, 25 Feb 2021 02:29:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 25 Feb 2021 02:29:29 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 25 Feb 2021 02:29:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 02:29:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:33:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 02:33:28 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:33:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 02:33:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 02:33:33 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 02:33:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 02:33:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 02:33:38 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 02:33:39 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 05:32:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 05:32:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 05:32:08 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 05:32:09 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 05:32:10 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 05:32:33 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 05:32:40 GMT
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
	-	`sha256:7325fd6c87e4ac3056b3e763f633c33fe16fafa49a53cddecd8e91c272a0ad44`  
		Last Modified: Thu, 25 Feb 2021 02:54:08 GMT  
		Size: 10.4 MB (10351227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b32babeb2a05f4d8ed07707937a77ccd9069f210d40429b161487521b4337d`  
		Last Modified: Thu, 25 Feb 2021 02:54:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192149405ed4fb55a866287392019b780c3bf456d69143a19922439d3fac9a5`  
		Last Modified: Thu, 25 Feb 2021 02:54:09 GMT  
		Size: 14.1 MB (14077047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b744f956d2311b4e86371412771b004bba688fe721896d73e82fe158499486`  
		Last Modified: Thu, 25 Feb 2021 02:54:05 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7901ee78194eba0a512fee3429a53027e6eab1c10e6fb5b686b67c3ae7e690`  
		Last Modified: Thu, 25 Feb 2021 02:54:05 GMT  
		Size: 16.9 KB (16891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a300ce7ec59c835da0d04c64bd6b3781ce71f7bb23bef366f7489f39d0def`  
		Last Modified: Thu, 25 Feb 2021 02:54:05 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ef38a3cdde7385dc35a84f21d69e9a6ed465af8abfb9c455e77b5b9da05b19`  
		Last Modified: Thu, 25 Feb 2021 05:38:56 GMT  
		Size: 2.9 MB (2871922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b42eebcc84e4974f671999b351589c5690a43c5519c64e674df084797aeb124`  
		Last Modified: Thu, 25 Feb 2021 05:38:55 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abbb1743266583b324f8ef63d9dd13f7e892e3239b3ea12ec79c79c92a6f8fe`  
		Last Modified: Thu, 25 Feb 2021 05:38:55 GMT  
		Size: 551.8 KB (551791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b12e752aa553969e81190ed56ce74b87e8e4bc645f4b70b683b41db25d0d8b`  
		Last Modified: Thu, 25 Feb 2021 05:38:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2399466576e7a77b5bbe3804a6673fe8beebda63c0aa7c6119441d4d044031`  
		Last Modified: Thu, 25 Feb 2021 05:39:03 GMT  
		Size: 18.8 MB (18819817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; 386

```console
$ docker pull drupal@sha256:df31f06c3ba45705e7f19c153630448a57f6049e4a47782ca607ce68a05ded75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51704844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3f2ba5d1e49a98f6fb049db58bcba098a6711e6b2a554acd323c4d2ccf7d9e`
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
# Wed, 24 Feb 2021 23:54:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 24 Feb 2021 23:54:27 GMT
ENV PHP_VERSION=7.4.15
# Wed, 24 Feb 2021 23:54:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Wed, 24 Feb 2021 23:54:28 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Wed, 24 Feb 2021 23:54:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 24 Feb 2021 23:54:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:01:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 00:01:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 00:01:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 00:01:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 00:01:04 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 00:01:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 00:01:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 00:01:06 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 00:01:06 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 02:38:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 02:38:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 02:38:48 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:38:48 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 02:38:48 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 02:39:00 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 02:39:01 GMT
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
	-	`sha256:3036a4850fc1b5e7bc43801f1635bcfbe962802747e51d0ac0334c6edea0d7a5`  
		Last Modified: Thu, 25 Feb 2021 00:44:31 GMT  
		Size: 10.4 MB (10351182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c919455c2a4867463701a8a0c3b0a5b021eaa146fcfd9acf5ccdb3023f2326ea`  
		Last Modified: Thu, 25 Feb 2021 00:44:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d4906856cdd772884fd42f7826a74bacb23378cf08a559fb44c01d2ac5af9c`  
		Last Modified: Thu, 25 Feb 2021 00:44:36 GMT  
		Size: 14.7 MB (14661057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbb9226b1f0ce23e6c4e85a9436741af5996ba40843804b92e0ebbfa46b8e8d`  
		Last Modified: Thu, 25 Feb 2021 00:44:30 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3c2463d8774db58d5344686036a0faeaa2bdc02350fc4bcbf0f748e4349bf7`  
		Last Modified: Thu, 25 Feb 2021 00:44:26 GMT  
		Size: 16.9 KB (16877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c767cd782120a8cd2c3aa329c0b5599f1df66da91d28e287ed7c99e5af2a29`  
		Last Modified: Thu, 25 Feb 2021 00:44:27 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7557e02edb7a9f446644e2a27f322cccc8a004a6f8f8ef86c4edc0619a2df7`  
		Last Modified: Thu, 25 Feb 2021 02:45:57 GMT  
		Size: 3.1 MB (3056823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40ed6463df9519f2389755400319b51ec0a2822d1c53c5cb021aac02c8fee95`  
		Last Modified: Thu, 25 Feb 2021 02:45:56 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1844022c813f3fbb2edc9ab8cb5773df697cff5ea824cbef9903edfaeb1e2d85`  
		Last Modified: Thu, 25 Feb 2021 02:45:56 GMT  
		Size: 551.8 KB (551786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2717046020aa14525001eb8a27ff52d85a0bdf67285482bcea02d2cd30929216`  
		Last Modified: Thu, 25 Feb 2021 02:45:56 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327ab008c0831fd36196df875a94b7509b85130f80c37e93f724fe8b7231cfc`  
		Last Modified: Thu, 25 Feb 2021 02:46:19 GMT  
		Size: 18.8 MB (18819598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; ppc64le

```console
$ docker pull drupal@sha256:3992e1ee8bfeab181c59d7e9f8f923a8bfa253f86966c10ed81e9619d61119cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52248589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad5627e8f7327bdb4f90bc3b708c9626eef3557d00df22db58fa4dc52bd50b9`
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
# Thu, 25 Feb 2021 02:37:54 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Feb 2021 02:37:56 GMT
ENV PHP_VERSION=7.4.15
# Thu, 25 Feb 2021 02:38:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 25 Feb 2021 02:38:08 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 25 Feb 2021 02:38:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 02:38:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:42:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 02:42:31 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 02:42:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 02:42:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 02:42:54 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 02:43:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 02:43:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 02:43:15 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 02:43:19 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 05:12:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 05:12:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 05:12:16 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 05:12:22 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 05:12:27 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 05:13:00 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 05:13:09 GMT
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
	-	`sha256:a2fd65a50eef1d1c6455ec6134dea48aa1a0da06551989ee2ec2206acb9ac3e8`  
		Last Modified: Thu, 25 Feb 2021 03:11:14 GMT  
		Size: 10.4 MB (10351222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27d17217306d57ef0ab74d1eb102123fba0803584e32ae07e62ba8400623954`  
		Last Modified: Thu, 25 Feb 2021 03:11:09 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d9dc098b26dcbae2cf4f8650c278d1249d87385882bbf35f62b7f4443b993`  
		Last Modified: Thu, 25 Feb 2021 03:11:13 GMT  
		Size: 15.3 MB (15255269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfe449e01b82e2a36427d11733f22f03017cb73cb5ce658b2c7468f8a89b277`  
		Last Modified: Thu, 25 Feb 2021 03:11:09 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b8232d6b41eb416cb2a5fea3f53e5dcfc7e3f4f0d83b6d149b8301ff5d1e56`  
		Last Modified: Thu, 25 Feb 2021 03:11:09 GMT  
		Size: 16.9 KB (16926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b724325c487081ded94ef91e3ce1c17469ba8cc9d0e5dcccfb574045365a6d93`  
		Last Modified: Thu, 25 Feb 2021 03:11:09 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05a8b64637c1ca82a6087352bbb258201511d559fd989eb23b76f2ef588554`  
		Last Modified: Thu, 25 Feb 2021 05:23:39 GMT  
		Size: 3.1 MB (3051796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09525a1c74b644539872e48e296163d53205001fd1818d8708bf86c67acdd6cf`  
		Last Modified: Thu, 25 Feb 2021 05:23:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0abf9d05746cb4c9e6f4381fe943536add566f385ea0257be5d48731311fc1bb`  
		Last Modified: Thu, 25 Feb 2021 05:23:39 GMT  
		Size: 551.8 KB (551789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7c1c4b410f30666cd01e92ef4d935a1dc1684916446620236e8df6905f0dc3`  
		Last Modified: Thu, 25 Feb 2021 05:23:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31450c1b7fbbe584ffc81cb004001c09b1e2e28105e37cfa85f03aaa9a923c49`  
		Last Modified: Thu, 25 Feb 2021 05:23:44 GMT  
		Size: 18.8 MB (18819294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.12` - linux; s390x

```console
$ docker pull drupal@sha256:fd1e9ad49bc5ab42bd40d6591629f4c5f52655f1f29344eb4a59e61146907073
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50178076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6783e56fd0016bb8315e0fa850cf5ff0707d3340b18496dc8f4f4e3b69a857`
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
# Thu, 25 Feb 2021 04:21:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Feb 2021 04:21:28 GMT
ENV PHP_VERSION=7.4.15
# Thu, 25 Feb 2021 04:21:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 25 Feb 2021 04:21:29 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 25 Feb 2021 04:21:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Feb 2021 04:21:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:27:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Feb 2021 04:27:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 25 Feb 2021 04:27:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Feb 2021 04:27:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Feb 2021 04:27:35 GMT
WORKDIR /var/www/html
# Thu, 25 Feb 2021 04:27:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 25 Feb 2021 04:27:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 25 Feb 2021 04:27:38 GMT
EXPOSE 9000
# Thu, 25 Feb 2021 04:27:39 GMT
CMD ["php-fpm"]
# Thu, 25 Feb 2021 06:42:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 25 Feb 2021 06:42:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 25 Feb 2021 06:42:15 GMT
COPY file:1b32c2cc2578adb470417567850eca1f7168281e86639ee273f7664dbafacc12 in /usr/local/bin/ 
# Thu, 25 Feb 2021 06:42:15 GMT
ENV DRUPAL_VERSION=9.1.4
# Thu, 25 Feb 2021 06:42:16 GMT
WORKDIR /opt/drupal
# Thu, 25 Feb 2021 06:42:45 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 25 Feb 2021 06:42:56 GMT
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
	-	`sha256:34d0a9f198dacdc35675318acc9f6cc2df4df0e4e0760ff56cb5caf41c218818`  
		Last Modified: Thu, 25 Feb 2021 04:55:26 GMT  
		Size: 10.4 MB (10351230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0539166d52fbd6eda6fbe3c786c9a414e5e210a6de94cc859a74211a6a546a2`  
		Last Modified: Thu, 25 Feb 2021 04:55:23 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a76a3216c799781feb407419484d53604ec823a60ea69e4fcaec22855f98d2`  
		Last Modified: Thu, 25 Feb 2021 04:55:27 GMT  
		Size: 13.6 MB (13569742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963f1a1609b1d6d82d62564c6345fbbff3ee9b38f3c7f5ada48c9f5ec372ea9f`  
		Last Modified: Thu, 25 Feb 2021 04:55:23 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d69551d428a56ab3419d0556aea362519001180b9328b591a3051b780b5bc`  
		Last Modified: Thu, 25 Feb 2021 04:55:23 GMT  
		Size: 16.9 KB (16888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d7d2b3a92af9a15e2f7a5a2a5bfd4f8d7baa79db1282e67493c855d65faebc`  
		Last Modified: Thu, 25 Feb 2021 04:55:23 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee38b5954fe2cdea48e2b34b90bec71b72bcbf1b6986802ee210ba914dbef7e`  
		Last Modified: Thu, 25 Feb 2021 06:49:24 GMT  
		Size: 2.9 MB (2905510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3a26f18896ebc5ac12e0f5d9f09eb77ee5f7226b3585f62822d2f4ff41cd41`  
		Last Modified: Thu, 25 Feb 2021 06:49:23 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debf5b8a9614e096056f511f524bd3a5a7c3bfd081165f3a1cb25373bc909ea`  
		Last Modified: Thu, 25 Feb 2021 06:49:24 GMT  
		Size: 551.8 KB (551791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87299ed74e43c490b325b167ed200339864d15d8cc3a4316ca2f307afa09cf7d`  
		Last Modified: Thu, 25 Feb 2021 06:49:24 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c592929e107dfb6fa213e49c55a11c81d4ea8667928595c35413a7cad317ba`  
		Last Modified: Thu, 25 Feb 2021 06:49:27 GMT  
		Size: 18.8 MB (18819625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
