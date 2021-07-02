## `drupal:9-php8.0-fpm-alpine3.13`

```console
$ docker pull drupal@sha256:cfc1d1674d7ca654f55f9d9d8d46c696a4dcf512ad9cb3648bb98fc44362d4db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `drupal:9-php8.0-fpm-alpine3.13` - linux; amd64

```console
$ docker pull drupal@sha256:f95e56a582ebcb7a1b9f2da0d39c141993a93c62002b13e19c9f9f348218daf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52872410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c58cb8c506f7e781894f5f3080012914bd2d99ab81b5d11188e679c2e556b02`
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
# Fri, 02 Jul 2021 00:21:28 GMT
ENV DRUPAL_VERSION=9.2.0
# Fri, 02 Jul 2021 00:21:28 GMT
WORKDIR /opt/drupal
# Fri, 02 Jul 2021 00:21:39 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 02 Jul 2021 00:21:41 GMT
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
	-	`sha256:2aa041fbf765cd0c0adb99822531de34a30bd31d6adb735e9bec396d66948c3e`  
		Last Modified: Fri, 02 Jul 2021 00:38:06 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f1e9f62b11a92d04475e1d493bc3e9a1ee2be413378a1550f4e8ec71891459`  
		Last Modified: Fri, 02 Jul 2021 00:38:11 GMT  
		Size: 19.2 MB (19157205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm variant v6

```console
$ docker pull drupal@sha256:e7ba847eefb67e7717151083109009551154dfa6c93218368635c8320fd04817
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50623285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f050a7b8f1b5fc15b706cee1eb07f2922b8f28619fd417ea5bc32c10ba23b448`
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
# Thu, 01 Jul 2021 23:10:31 GMT
ENV DRUPAL_VERSION=9.2.0
# Thu, 01 Jul 2021 23:10:31 GMT
WORKDIR /opt/drupal
# Thu, 01 Jul 2021 23:10:59 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Jul 2021 23:11:00 GMT
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
	-	`sha256:49907948ba7003b49f6b017002f1159c0db9d2908fb3ada4f4e60b548c00f4d5`  
		Last Modified: Thu, 01 Jul 2021 23:27:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbd35a4b063b136f2cd0ccf07c409b050649ce3a0dca707faf67f7c5fc52ab4`  
		Last Modified: Thu, 01 Jul 2021 23:27:31 GMT  
		Size: 19.2 MB (19157223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm variant v7

```console
$ docker pull drupal@sha256:a547027662cb65745df03899ff66846acff20e4ae9f635dac7191ea2808e19dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49240994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce732ce957e6843f7392c7a5ba67c4ab0031bc59da8ecf89ec9c2d8cbe27359`
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
# Fri, 02 Jul 2021 02:21:37 GMT
ENV DRUPAL_VERSION=9.2.0
# Fri, 02 Jul 2021 02:21:37 GMT
WORKDIR /opt/drupal
# Fri, 02 Jul 2021 02:22:03 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 02 Jul 2021 02:22:06 GMT
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
	-	`sha256:f0f73d00934e74823e143a8029541687b60e9facd5bb2577f77d3eaa54636537`  
		Last Modified: Fri, 02 Jul 2021 03:02:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fddbd5df8d22e48006862c09581ae6c541eb452b16f4a808b7579ec04c5370`  
		Last Modified: Fri, 02 Jul 2021 03:03:20 GMT  
		Size: 19.2 MB (19156998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:1de6eb21f8b41fd27a1d0caf2818a4bcd68ba06f91e725e4b53a7be0a32b6309
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51638985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84226222299084b122dd9864b4f7a072be98b3b2523a323e446bd08f72ab6d14`
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
# Thu, 01 Jul 2021 23:01:24 GMT
ENV DRUPAL_VERSION=9.2.0
# Thu, 01 Jul 2021 23:01:24 GMT
WORKDIR /opt/drupal
# Thu, 01 Jul 2021 23:01:33 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Jul 2021 23:01:35 GMT
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
	-	`sha256:54572e22b46ec6dfc1ea2ec57be3d955a3bc1588bed3addcf1c164a8fc625813`  
		Last Modified: Thu, 01 Jul 2021 23:23:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e306c63dadcac8cbc31fecbec6ffb8a1d6de5f88ada46221a9b7372ecbdc4edc`  
		Last Modified: Thu, 01 Jul 2021 23:23:43 GMT  
		Size: 19.2 MB (19157014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; 386

```console
$ docker pull drupal@sha256:5f83ca0da2a2fbb42a8350561fdbaf7b6806d818001557c9414440a3d917cc30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53458333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2475b3677b08083ab81246ad28a082751ccf53782ed685457f554861e9f8a89f`
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
# Fri, 02 Jul 2021 00:45:03 GMT
ENV DRUPAL_VERSION=9.2.0
# Fri, 02 Jul 2021 00:45:03 GMT
WORKDIR /opt/drupal
# Fri, 02 Jul 2021 00:45:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 02 Jul 2021 00:45:18 GMT
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
	-	`sha256:35ef02554bf89b81f61c6263e7320ffee1e8d5258bc10d523c07c2ff12861b54`  
		Last Modified: Fri, 02 Jul 2021 01:09:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4b18003ddd870cb80ed5ae86654ebd5572e6112f79961496098a79d620deb4`  
		Last Modified: Fri, 02 Jul 2021 01:09:19 GMT  
		Size: 19.2 MB (19157070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.13` - linux; s390x

```console
$ docker pull drupal@sha256:e31c4c38a07b370f22116738c825e28d25d88c5f91a1a674843d381cfb9dd0bb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51316265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a98c5d2e01d021e0c637de788bb98df9ed729c83ee63304f711a3e2d47d3a2`
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
# Sat, 26 Jun 2021 00:58:31 GMT
ENV PHP_VERSION=8.0.7
# Sat, 26 Jun 2021 00:58:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Sat, 26 Jun 2021 00:58:31 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 19:41:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 28 Jun 2021 19:41:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:45:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 19:45:31 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:45:33 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 19:45:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 19:45:34 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 19:45:35 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Mon, 28 Jun 2021 19:45:36 GMT
STOPSIGNAL SIGQUIT
# Mon, 28 Jun 2021 19:45:36 GMT
EXPOSE 9000
# Mon, 28 Jun 2021 19:45:36 GMT
CMD ["php-fpm"]
# Thu, 01 Jul 2021 00:54:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Jul 2021 00:54:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Jul 2021 00:54:38 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Thu, 01 Jul 2021 00:54:39 GMT
ENV DRUPAL_VERSION=9.2.0
# Thu, 01 Jul 2021 00:54:40 GMT
WORKDIR /opt/drupal
# Thu, 01 Jul 2021 00:55:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Jul 2021 00:55:21 GMT
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
	-	`sha256:b2281845ca6d30f401d8b8abd763e43542b7634138bf92f2fe2426136b47f05f`  
		Last Modified: Mon, 28 Jun 2021 21:08:03 GMT  
		Size: 10.8 MB (10788571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70003a4ba09255ee83f9202bedbc599bd547db299248a50d375208c69294d162`  
		Last Modified: Mon, 28 Jun 2021 21:08:01 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85abe529ab0ac676654a72cfee0fd0046619fe94c1b38fa87aaa20dead58450`  
		Last Modified: Mon, 28 Jun 2021 21:08:03 GMT  
		Size: 14.5 MB (14451230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cca694f17ba27a8ae4cdc323deebbbe61de23afab0c323300dc579a20b0db93`  
		Last Modified: Mon, 28 Jun 2021 21:08:00 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17f100d8b0eb61c8924f858e47bec1726d14f35d68dc11c55ae0cfe6d905990`  
		Last Modified: Mon, 28 Jun 2021 21:08:01 GMT  
		Size: 17.6 KB (17606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25351cfec8c043db6c2a075ee8a11e9373ee82391ba18835bf04f5d869d15da5`  
		Last Modified: Mon, 28 Jun 2021 21:08:01 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19e5a16ef43d7c045dd3bf5dd1a4fcc87328f9c0cdbd8abc3ec82ea52f2dcf5`  
		Last Modified: Thu, 01 Jul 2021 01:41:46 GMT  
		Size: 2.0 MB (1965633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6dfbfb205e38220cd15bbb6a35787841e3344b76e6ed79e995b10e06bc6925`  
		Last Modified: Thu, 01 Jul 2021 01:41:46 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c638a0cdc751667b9942ec23e50bcf81e04ebfb0ec983f33d802a11b87ce510c`  
		Last Modified: Thu, 01 Jul 2021 01:41:50 GMT  
		Size: 553.2 KB (553180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a28c8a0830596b7dad3030f68e86d36fcb5717c240b5d6a42e41c988f75b2`  
		Last Modified: Thu, 01 Jul 2021 01:41:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d647c4df469c1d4f9c709a9921abde6b8faf150d71df73344cd5dd14106e78e`  
		Last Modified: Thu, 01 Jul 2021 01:41:50 GMT  
		Size: 19.2 MB (19156824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
