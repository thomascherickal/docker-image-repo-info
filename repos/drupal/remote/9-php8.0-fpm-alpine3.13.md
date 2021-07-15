## `drupal:9-php8.0-fpm-alpine3.13`

```console
$ docker pull drupal@sha256:36093c48dcd3ec15aa40d24f3dd2ed50ca3ae10af3e004f3922f803212b0f010
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

### `drupal:9-php8.0-fpm-alpine3.13` - linux; amd64

```console
$ docker pull drupal@sha256:22000fa0868a7db29cfb48b8c617c8e60d07ed491cc38e5cc150d97259e5b555
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52890682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22dc37aff3120c30c1c1ee13d968b1425fb0e887768c421cf21e3b1ea5d94dd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:08:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 23:06:52 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 23:06:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 23:06:52 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 23:06:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Jul 2021 23:06:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:16:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 23:16:49 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:16:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 23:16:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 23:16:51 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 23:16:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Jul 2021 23:16:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jul 2021 23:16:53 GMT
EXPOSE 9000
# Thu, 01 Jul 2021 23:16:53 GMT
CMD ["php-fpm"]
# Fri, 02 Jul 2021 00:21:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Jul 2021 00:21:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Jul 2021 00:21:28 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:20:44 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 18:20:44 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 18:20:54 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 18:20:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9aa845cf275bf131b4534c530b6c6382b4d28e0acaa81491dbae8f132b112`  
		Last Modified: Thu, 01 Jul 2021 23:27:10 GMT  
		Size: 10.7 MB (10693959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb827bec5b1dd5b330649895a6e16d68de57b0dae7bb516eb0a4ee64575a5733`  
		Last Modified: Thu, 01 Jul 2021 23:27:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e85085ed11a39587a78108300e2ab408f773fadfe4bb5c210c31b0e457fbc54`  
		Last Modified: Thu, 01 Jul 2021 23:27:11 GMT  
		Size: 15.7 MB (15658697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6306c01fd24bfb23e526136d76d51a8e5d58c823277ee0214b17519094245d71`  
		Last Modified: Thu, 01 Jul 2021 23:27:07 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69574e632d7dd1abde610f701e4aafa4d565a9596751ef77d8471e7480536737`  
		Last Modified: Thu, 01 Jul 2021 23:27:07 GMT  
		Size: 17.6 KB (17642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22426c5ae2042ee2bc2b660d9af4fd93aa9c6669c15ed4f57f0423ae23fe2767`  
		Last Modified: Thu, 01 Jul 2021 23:27:07 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b271b3ef58227bb8ecb23e4ce4853dae52b5fe51c34a280d078b1a8419eea3`  
		Last Modified: Fri, 02 Jul 2021 00:38:07 GMT  
		Size: 2.3 MB (2264232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be7498834c1ccb0136b2f57a2c5bdaa5a0681efae913b00aa2e93229b1be1f`  
		Last Modified: Fri, 02 Jul 2021 00:38:06 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1647873a968e26aa8426304a95528d919536cbfa875917dae0543dba32b360c`  
		Last Modified: Fri, 02 Jul 2021 00:38:06 GMT  
		Size: 553.2 KB (553181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5525214d9f0551a7e78847247bb8b2e4e8297316d9a5f7830a4a2fbe06751712`  
		Last Modified: Thu, 08 Jul 2021 18:29:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5c26f56c02a2946f94646b42795ae983808744b3477dfa1248b9021947cfa5`  
		Last Modified: Thu, 08 Jul 2021 18:29:24 GMT  
		Size: 19.2 MB (19175475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm variant v6

```console
$ docker pull drupal@sha256:eaa547d2c715db00a287eb2c0d3ba2b71de7bfcb4c5c74269894dd9be3d03440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50641978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c688b21d8369ba595b0a9fe579c7e64da7fb5f0697e5a5e42f94527229df7a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Fri, 25 Jun 2021 20:35:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 25 Jun 2021 20:35:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 25 Jun 2021 20:35:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 25 Jun 2021 20:35:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 25 Jun 2021 20:35:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 25 Jun 2021 20:41:07 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 25 Jun 2021 20:41:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 25 Jun 2021 20:41:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 25 Jun 2021 20:41:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 25 Jun 2021 21:01:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 20:59:00 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 20:59:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 20:59:01 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 20:59:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Jul 2021 20:59:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:04:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 21:04:17 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Jul 2021 21:04:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 21:04:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 21:04:21 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 21:04:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Jul 2021 21:04:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jul 2021 21:04:23 GMT
EXPOSE 9000
# Thu, 01 Jul 2021 21:04:24 GMT
CMD ["php-fpm"]
# Thu, 01 Jul 2021 23:10:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Jul 2021 23:10:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Jul 2021 23:10:30 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:52:53 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 18:52:53 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 18:53:20 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 18:53:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02730f7552a0de248d6493757a223e50176748f63ad0bba2a64bb38ed28c2b94`  
		Last Modified: Fri, 25 Jun 2021 22:16:05 GMT  
		Size: 1.7 MB (1696010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff392e05204a68478ef0a2b90630d1d3c5debc169e1284b3e1d0479ba261fef`  
		Last Modified: Fri, 25 Jun 2021 22:16:04 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add406debd836764089aff049af45ac26fb9cc2e3b6614db1a2396f41b1728db`  
		Last Modified: Fri, 25 Jun 2021 22:16:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efca7e5a31d85e8efcd5f4baa6314c69dd1f8d2c0d3c209d19269d619116d25f`  
		Last Modified: Thu, 01 Jul 2021 21:18:01 GMT  
		Size: 10.7 MB (10693953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a6fac2e07650dddc9c561dcd8a54ed00d952f7d79ab431e467cc8f8c0f498d`  
		Last Modified: Thu, 01 Jul 2021 21:17:57 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3b3cd1c05cd99f0475bde4cf09a56157674f71e465dbb2419d845a43fa518e`  
		Last Modified: Thu, 01 Jul 2021 21:18:08 GMT  
		Size: 14.1 MB (14054715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6a37862a483bfd281ae0239f8ef850cd928e42e8b62758335deaee225d13b5`  
		Last Modified: Thu, 01 Jul 2021 21:17:57 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c2fef978065b0ef8647ea4c95127d20ab98d919b8b3992eaa97fa389b05f0b`  
		Last Modified: Thu, 01 Jul 2021 21:17:57 GMT  
		Size: 17.6 KB (17595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0725f5c978595c8d51867f0f69018cdf4fc608c0ddb030f7e7c28a1d7ba49`  
		Last Modified: Thu, 01 Jul 2021 21:17:57 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615ea7cb630a15b3b21d9a71446da51b7d0e3f6d4ca5d089ee4fb1bb977f062e`  
		Last Modified: Thu, 01 Jul 2021 23:27:03 GMT  
		Size: 1.8 MB (1815137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63a9e3b2e2d0fe049b9861a3a3d8d13bb16d0098062f1b797139c34573e0639`  
		Last Modified: Thu, 01 Jul 2021 23:27:02 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573259efd2679f5918af6aee011ba2ac29571af38d93727626c3831b43e8add7`  
		Last Modified: Thu, 01 Jul 2021 23:27:02 GMT  
		Size: 553.2 KB (553180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba64ad1b9fde26e2e32b8d7f6745b6d190532effee6895ba19c075902f308`  
		Last Modified: Thu, 08 Jul 2021 19:03:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb8cd5316fa78bb540edc1499d8c44ea04e78a35a501f4d0e88ef1a4b640937`  
		Last Modified: Thu, 08 Jul 2021 19:03:42 GMT  
		Size: 19.2 MB (19175916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0bf4040130e6f05569347e3e83b318f193bbf9ef1cf3ad18ad4662d07ad639b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49259758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ff08adb651d398de8f959ca0232aa151cdd1651a1230de7a77c45602c3b198`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 23 Jun 2021 08:51:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Jun 2021 08:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Jun 2021 08:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Jun 2021 08:52:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:52:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:56:45 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 23 Jun 2021 08:56:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:56:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:56:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:35:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 23:15:40 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 23:15:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 23:15:41 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 23:15:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Jul 2021 23:15:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:19:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 23:20:01 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Jul 2021 23:20:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 23:20:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 23:20:04 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 23:20:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Jul 2021 23:20:06 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jul 2021 23:20:06 GMT
EXPOSE 9000
# Thu, 01 Jul 2021 23:20:07 GMT
CMD ["php-fpm"]
# Fri, 02 Jul 2021 02:21:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Jul 2021 02:21:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Jul 2021 02:21:37 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 20:37:45 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 20:37:46 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 20:38:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 20:38:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21d8017ada758170e7d9cedcdbcb8ed0db8f51ee7e74bde3d216e2ec00c8f4`  
		Last Modified: Wed, 23 Jun 2021 11:54:48 GMT  
		Size: 1.6 MB (1563945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cb28ec7ce662715805a4e324ca33a9c761171d7140aeb837cba3507ec56da`  
		Last Modified: Wed, 23 Jun 2021 11:54:47 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b3422092a8218116e5bc11a213aca134b09fa4f008686f110cb93d480f070c`  
		Last Modified: Wed, 23 Jun 2021 11:54:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba58317067f307ac139c72952a61b122941227c0d6039f0062c9f7f8a85b08ea`  
		Last Modified: Thu, 01 Jul 2021 23:48:32 GMT  
		Size: 10.7 MB (10693959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3325f1bdcbfbe6cac98bbc562b29d2b9bf15f7205d343b8ad48f07d18ee88a`  
		Last Modified: Thu, 01 Jul 2021 23:48:27 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85faf2edd4922a34d207d45443d9d4f7a40090d569cf9fc5e33ff5539caf57f4`  
		Last Modified: Thu, 01 Jul 2021 23:48:37 GMT  
		Size: 13.2 MB (13170805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7e82354e2a83f915a2be465140d93b41e0f4b14d4e32f94b523fafed30d3a2`  
		Last Modified: Thu, 01 Jul 2021 23:48:27 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145f7f04312597c9b01a5b06481502b352b1ebd3fbe2dd04eef5c17fac879653`  
		Last Modified: Thu, 01 Jul 2021 23:48:27 GMT  
		Size: 17.6 KB (17599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb6e9b16c0ddd11b6c0ced98b60dc9b5b1190543f70921083d13f2c04817d0c`  
		Last Modified: Thu, 01 Jul 2021 23:48:27 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d796c0a7805d59a23468c2ba673a4bc4cfbab6b43da3221cba12c36de2f23ee0`  
		Last Modified: Fri, 02 Jul 2021 03:02:51 GMT  
		Size: 1.6 MB (1647027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c9791f8a1ea56658d78e2aecd076812e13129b4607ad6c1a01aed33263a98f`  
		Last Modified: Fri, 02 Jul 2021 03:02:50 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a9a36e62bfbad66f97b2f89e4884c464d7d6b02f5acd8ef046106a5ea4271f`  
		Last Modified: Fri, 02 Jul 2021 03:02:51 GMT  
		Size: 553.2 KB (553180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15762548a2a1ab7cd6cdac2c08ae5f32ca81ba153ee809c73c0aeca4f0ab7481`  
		Last Modified: Thu, 08 Jul 2021 21:05:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33be869bbf43c926ce577f81b8ee4717c2b186657abe1921e55e84ea11ae747`  
		Last Modified: Thu, 08 Jul 2021 21:05:38 GMT  
		Size: 19.2 MB (19175762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:6333d8e743b3c0805c3db5d7ddab22b3bb28d5681fa91a08b745158033107d21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51657913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3404b90259e7cc77a1d1c289135ecac43404221f3fcfe3a43afeaf4fdfa01d97`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 06:30:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 16 Jun 2021 06:30:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 16 Jun 2021 06:30:51 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 16 Jun 2021 06:30:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 16 Jun 2021 06:30:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 16 Jun 2021 06:38:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 16 Jun 2021 07:04:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Jul 2021 22:23:18 GMT
ENV PHP_VERSION=8.0.8
# Thu, 01 Jul 2021 22:23:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 01 Jul 2021 22:23:19 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 01 Jul 2021 22:23:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Jul 2021 22:23:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:28:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Jul 2021 22:28:21 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Jul 2021 22:28:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Jul 2021 22:28:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Jul 2021 22:28:23 GMT
WORKDIR /var/www/html
# Thu, 01 Jul 2021 22:28:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Jul 2021 22:28:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jul 2021 22:28:24 GMT
EXPOSE 9000
# Thu, 01 Jul 2021 22:28:24 GMT
CMD ["php-fpm"]
# Thu, 01 Jul 2021 23:01:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Jul 2021 23:01:23 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Jul 2021 23:01:24 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:41:29 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 18:41:29 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 18:41:39 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 18:41:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc18e501d273a5dcc26bc1081722d23265e91017730cc8d28538506985fbfae`  
		Last Modified: Wed, 16 Jun 2021 08:22:48 GMT  
		Size: 1.7 MB (1710127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cae51f9170182c26896b8887cec72ef02fc7a6ee745b63f2d5205fd4d2d1a9`  
		Last Modified: Wed, 16 Jun 2021 08:22:46 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fa7f9524184404473a9920618e9aa956decfca08f5ccdd2a9b83aa9c564a03`  
		Last Modified: Wed, 16 Jun 2021 08:22:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1298df59c2da675fed15a5ad52730052f7e7746ec1c609ebd5a012d75316b16b`  
		Last Modified: Thu, 01 Jul 2021 22:44:11 GMT  
		Size: 10.7 MB (10693974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabec0825f49e67528ec973e6d7445ad23f0331362f1a5c08d538e9148674acf`  
		Last Modified: Thu, 01 Jul 2021 22:44:08 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bfd8c5759fa8040a46190a51892b9391ae6d2ec2d1963eb3bb70e58efdeaa5`  
		Last Modified: Thu, 01 Jul 2021 22:44:11 GMT  
		Size: 14.9 MB (14857122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a256193620a777fdd6fd8beb6ea71a03541a3852c5d8b966cedee0dfdb8dc5`  
		Last Modified: Thu, 01 Jul 2021 22:44:08 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c8c10e5578dab0ddaaf6c2fc39c1bfd9ed054dad365c3aa59db21dffa7cbc`  
		Last Modified: Thu, 01 Jul 2021 22:44:08 GMT  
		Size: 17.6 KB (17604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85934bd001ba9d98d21a2738d6105b7e43d5c8ce80e108afb94a728989bf9273`  
		Last Modified: Thu, 01 Jul 2021 22:44:08 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8110c2476d4fc6f3f92518f3acc7e690576993c4c7031509e1ee493683b6e1`  
		Last Modified: Thu, 01 Jul 2021 23:23:39 GMT  
		Size: 1.9 MB (1924603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f125aea4d0a907402bdf5329ec7a588491763ca697608d50ef29879b62676192`  
		Last Modified: Thu, 01 Jul 2021 23:23:38 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d8f38000c2d181a14fb820411d031d0a0dbf8028720c72434d9038c6a77f72`  
		Last Modified: Thu, 01 Jul 2021 23:23:38 GMT  
		Size: 553.2 KB (553179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdc03f9c791358d386b373b7da7376d067498720179e0b024690a83170371d5`  
		Last Modified: Thu, 08 Jul 2021 18:56:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60d630429b4b10510cce177771e3710b2df36665d698a43541f8966f2f3a1b`  
		Last Modified: Thu, 08 Jul 2021 18:56:28 GMT  
		Size: 19.2 MB (19175942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; 386

```console
$ docker pull drupal@sha256:3fabf8f575a59e5593b96601bfbc13a6cb908b469b551bafe5a4fe3914b718f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53477115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb8179d18411af358904dd41d4d96be15b2884dbdd78171489bf20b3b9db6d70`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:45:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:45:36 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 02 Jul 2021 00:04:06 GMT
ENV PHP_VERSION=8.0.8
# Fri, 02 Jul 2021 00:04:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Fri, 02 Jul 2021 00:04:06 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Fri, 02 Jul 2021 00:04:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 02 Jul 2021 00:04:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 02 Jul 2021 00:11:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 02 Jul 2021 00:11:18 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 02 Jul 2021 00:11:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 02 Jul 2021 00:11:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 02 Jul 2021 00:11:20 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 00:11:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 02 Jul 2021 00:11:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Jul 2021 00:11:21 GMT
EXPOSE 9000
# Fri, 02 Jul 2021 00:11:21 GMT
CMD ["php-fpm"]
# Fri, 02 Jul 2021 00:45:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Jul 2021 00:45:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Jul 2021 00:45:02 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:40:35 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 18:40:35 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 18:40:50 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 18:40:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67aca29f694b185dedb1433bcd696d4d3ffc705c376c5fe88a49eeceaaa5dc5a`  
		Last Modified: Fri, 02 Jul 2021 00:28:49 GMT  
		Size: 10.7 MB (10693938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bb2105e2e465ae4dc0d1923210b2a06a506f494420af08bd044f79b24d6e2a`  
		Last Modified: Fri, 02 Jul 2021 00:28:46 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87db694c35a94dd3f737e9f533dad064a672ee3c7b1e4752380689d10a6e2c32`  
		Last Modified: Fri, 02 Jul 2021 00:28:50 GMT  
		Size: 16.0 MB (16036084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e230c7759075fa6cd0ab55d1203517ffd04e4362ef864a44736b6ae2d7dc8016`  
		Last Modified: Fri, 02 Jul 2021 00:28:46 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf0ecf3a5ae14a544a00555dd073cd3a17229cac2ec40232a4a7e09168396e4`  
		Last Modified: Fri, 02 Jul 2021 00:28:45 GMT  
		Size: 17.6 KB (17628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f185596b3fc1383b80a02416c5ae26e3b08b289f72c5ba1bb84a9f83a2966`  
		Last Modified: Fri, 02 Jul 2021 00:28:45 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a0206db0f36a36f6492c6f0db02851526a4ecbf2858cf14fda147d8cef909d`  
		Last Modified: Fri, 02 Jul 2021 01:09:05 GMT  
		Size: 2.4 MB (2368917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e40fb85f1d1403b6df33d1970d9cff27a7d83250e2f2fde5cc563f1661ef7c`  
		Last Modified: Fri, 02 Jul 2021 01:09:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1cf449426e4fff841ca6cefc5809cfaa8c0b38f1feb907a120f229177a03e`  
		Last Modified: Fri, 02 Jul 2021 01:09:05 GMT  
		Size: 553.2 KB (553182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0973cc8bd4f95065f395ac51fc8d345d14a3d2cf8066d2ce5df975ce65b9b9`  
		Last Modified: Thu, 08 Jul 2021 18:56:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82ff39fc478a6dbcb4454d28bbcf01d808683a1c83755a35d6e03a24f4e4fdd`  
		Last Modified: Thu, 08 Jul 2021 18:56:33 GMT  
		Size: 19.2 MB (19175852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; ppc64le

```console
$ docker pull drupal@sha256:168790ebdeb0c4f674496cc7fcb5de58aabae74667b13cb17439b231b1b42da1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53287365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb4a6aae985da56c37f357c36753ed3192ba46784b010001cc83709c30c5d22`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:20:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 26 Jun 2021 05:20:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 26 Jun 2021 05:20:42 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 26 Jun 2021 05:20:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 05:21:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 05:31:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 26 Jun 2021 05:31:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 05:31:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 05:31:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 06:33:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 08 Jul 2021 14:46:17 GMT
ENV PHP_VERSION=8.0.8
# Thu, 08 Jul 2021 14:46:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Thu, 08 Jul 2021 14:46:34 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Thu, 08 Jul 2021 14:47:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 08 Jul 2021 14:47:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 08 Jul 2021 14:51:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 08 Jul 2021 14:52:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 08 Jul 2021 14:52:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 08 Jul 2021 14:52:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 08 Jul 2021 14:52:28 GMT
WORKDIR /var/www/html
# Thu, 08 Jul 2021 14:52:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 08 Jul 2021 14:52:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 08 Jul 2021 14:52:53 GMT
EXPOSE 9000
# Thu, 08 Jul 2021 14:52:57 GMT
CMD ["php-fpm"]
# Fri, 09 Jul 2021 00:46:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 09 Jul 2021 00:46:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 09 Jul 2021 00:46:21 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Fri, 09 Jul 2021 00:46:26 GMT
ENV DRUPAL_VERSION=9.2.1
# Fri, 09 Jul 2021 00:46:43 GMT
WORKDIR /opt/drupal
# Fri, 09 Jul 2021 00:47:27 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 09 Jul 2021 00:47:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f951a2e70106ea34807c15a04b82f820f926288e94bd676ac52db812bc8373`  
		Last Modified: Sat, 26 Jun 2021 09:07:32 GMT  
		Size: 1.8 MB (1753168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73a8f22ea03b3d4d02e89825955b8559ca88f753dd23eaaa5076e4a251bf1e`  
		Last Modified: Sat, 26 Jun 2021 09:07:32 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45bd3fedd9fb06be753e4fae6edacd9ce7176b7fe89309de224e925fb94d33b`  
		Last Modified: Sat, 26 Jun 2021 09:07:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78513ba021bb260e94341e70ae1f8f2ad10d01ba0c203cf025b93fbde0314cb8`  
		Last Modified: Thu, 08 Jul 2021 17:09:31 GMT  
		Size: 10.7 MB (10693948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fd6c68e6fffbc9a97a056f6989f0ef31b87f402416e4c672d04eec3112d932`  
		Last Modified: Thu, 08 Jul 2021 17:09:27 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4505a9f9b1c983502a6294471e9fc0225e13c356bd137e193258344b3a4d61e`  
		Last Modified: Thu, 08 Jul 2021 17:09:31 GMT  
		Size: 16.2 MB (16159338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cc9116bc9d8ab1212b25caa772f35146ad7f8627323338ad37ca6894fb8fc8`  
		Last Modified: Thu, 08 Jul 2021 17:09:27 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fd48b453bdc047464761939d1152c1fb283520b8ba3ba08073e0be946c8fe8`  
		Last Modified: Thu, 08 Jul 2021 17:09:27 GMT  
		Size: 17.6 KB (17604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96d74768e1d252c7b52afdad22cc8068c46388085be902a85d77ca9eef8fbc0`  
		Last Modified: Thu, 08 Jul 2021 17:09:27 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240b2d5a0d53037005d7ee09e936675de2bfdaa75c36c7e259ece6d50e8888c`  
		Last Modified: Fri, 09 Jul 2021 01:34:33 GMT  
		Size: 2.1 MB (2107902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0372989d48217d3f09dc3f51f8b7c316740b264e43f0c59274bfb3943b11eb64`  
		Last Modified: Fri, 09 Jul 2021 01:34:32 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e377c4089128c3aaafd0ff6450473bc876dfecc7a87edbd270878df6bb82aa64`  
		Last Modified: Fri, 09 Jul 2021 01:34:32 GMT  
		Size: 553.2 KB (553185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5cd1e4755e3e215bb356bfb4b1c041e4c0a9f3548cc2515dd07ea020cafdcb`  
		Last Modified: Fri, 09 Jul 2021 01:34:32 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31f58490baca1a18d0bd3a72286c0f6976fc8bb5c4dfb92809afe4a945cf7a6`  
		Last Modified: Fri, 09 Jul 2021 01:36:57 GMT  
		Size: 19.2 MB (19175728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; s390x

```console
$ docker pull drupal@sha256:a54e3c803bb304c867b30b192dd523f9206e1d3552825d24ce2e11833477a19b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51242172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc43e672eb69c117377365cd6ab26d40d9fb01b7c73ac586069a7987ae909ef1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 00:28:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 26 Jun 2021 00:28:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 26 Jun 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 26 Jun 2021 00:28:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 00:28:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 00:32:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 26 Jun 2021 00:32:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:32:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:32:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 00:58:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 02 Jul 2021 00:29:15 GMT
ENV PHP_VERSION=8.0.8
# Fri, 02 Jul 2021 00:29:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.8.tar.xz.asc
# Fri, 02 Jul 2021 00:29:16 GMT
ENV PHP_SHA256=dc1668d324232dec1d05175ec752dade92d29bb3004275118bc3f7fc7cbfbb1c
# Fri, 02 Jul 2021 00:30:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 02 Jul 2021 00:30:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 02 Jul 2021 00:36:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 02 Jul 2021 00:36:06 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 02 Jul 2021 00:36:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 02 Jul 2021 00:36:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 02 Jul 2021 00:36:15 GMT
WORKDIR /var/www/html
# Fri, 02 Jul 2021 00:36:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 02 Jul 2021 00:36:17 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Jul 2021 00:36:18 GMT
EXPOSE 9000
# Fri, 02 Jul 2021 00:36:18 GMT
CMD ["php-fpm"]
# Fri, 02 Jul 2021 02:53:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Jul 2021 02:53:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Jul 2021 02:53:13 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:43:30 GMT
ENV DRUPAL_VERSION=9.2.1
# Thu, 08 Jul 2021 18:43:31 GMT
WORKDIR /opt/drupal
# Thu, 08 Jul 2021 18:43:43 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 08 Jul 2021 18:43:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be2b8fee15de15cad265ec16cd90845ce0596ebefefc22db3a00d5d628dd9e5`  
		Last Modified: Sat, 26 Jun 2021 02:20:08 GMT  
		Size: 1.8 MB (1767237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5836809602f37cefd11e6e0f52773bf771e6d9706874af78ee4a1d01ba5790`  
		Last Modified: Sat, 26 Jun 2021 02:20:07 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56f0b7af5c8e25cd9180f6340dc69ba4b4d35f5807e27aed1617a1c2c5ed055`  
		Last Modified: Sat, 26 Jun 2021 02:20:07 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86903dec41e3a8719454be157372247ffe6db2c691c81b2e68a591d360f4fac`  
		Last Modified: Fri, 02 Jul 2021 01:35:27 GMT  
		Size: 10.7 MB (10693960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5c5aec6df1361fb3a8a621b73d7d1f04891f5bacdeb68980255d2610b859b5`  
		Last Modified: Fri, 02 Jul 2021 01:35:17 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583675ee1c85bc377ca17f38298392c31e1f3981713bcab5b0d98e7770369470`  
		Last Modified: Fri, 02 Jul 2021 01:35:17 GMT  
		Size: 14.5 MB (14452610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f25b4aae18b84aabd1d4dcd98442818df2ecae1b943f5345f2782041f0e311`  
		Last Modified: Fri, 02 Jul 2021 01:35:13 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679fc69b9723c6fc59e205a662a2295507aa05b8a51b92a290db4603096cb696`  
		Last Modified: Fri, 02 Jul 2021 01:35:13 GMT  
		Size: 17.6 KB (17605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560c60de2db8946d80be38dcd1ba8e7a5cfcb7a875d18cfdf0cf6bba2db99fbf`  
		Last Modified: Fri, 02 Jul 2021 01:35:13 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e670a04c11c19e90501a57827c83402abb592a9ccd0e70d4ee1f4c80c90112`  
		Last Modified: Fri, 02 Jul 2021 04:07:57 GMT  
		Size: 2.0 MB (1965676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ae30708fbf7ddb563290496b32e7a18b1de296920158c904586ab9fb1f0bf6`  
		Last Modified: Fri, 02 Jul 2021 04:07:57 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931dd0b327d440d3f90d8b2f8a4174863d9f17b2f79fce6357bb27d690a1303a`  
		Last Modified: Fri, 02 Jul 2021 04:07:57 GMT  
		Size: 553.2 KB (553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8320d3c5e490b7901cc73d0b888bb1a7080a120fe78cff8a9a5842239c9a336`  
		Last Modified: Thu, 08 Jul 2021 18:54:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbb89f7efd697c703a8272aaf91a60d3359a220a68deba72ebbcae963819ac4`  
		Last Modified: Thu, 08 Jul 2021 18:54:35 GMT  
		Size: 19.2 MB (19175901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
