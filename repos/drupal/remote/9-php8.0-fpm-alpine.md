## `drupal:9-php8.0-fpm-alpine`

```console
$ docker pull drupal@sha256:b0a6331db5360ac3ae17e1976896ac57a1eacd44ac17a6884ead6810c8264f24
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

### `drupal:9-php8.0-fpm-alpine` - linux; amd64

```console
$ docker pull drupal@sha256:ebbc2d93b22ad8a8454e75139745cbea371d1959c617be95f93c83fb4a0dbb71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52599288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af87d91d4fc1e19ed4818400f96b11331304744a30a2d855c88070881a213a29`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:20:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:20:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:20:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:20:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:20:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:30:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:30:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:30:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:30:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:30:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 21:03:15 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 21:03:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 21:03:15 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 21:03:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 21:03:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 21:08:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 21:08:56 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 21:08:58 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 21:08:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 21:08:58 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 21:09:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 21:09:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 21:09:00 GMT
EXPOSE 9000
# Fri, 07 May 2021 21:09:00 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 21:38:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 21:38:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 21:38:27 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 21:38:27 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 21:38:27 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 21:38:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 21:38:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a078c9cf1904c807a7567f1e8845b68ff4d8a3a58f3c1e7263248f7503b7ca4`  
		Last Modified: Thu, 15 Apr 2021 02:17:07 GMT  
		Size: 1.4 MB (1369201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7a9502060da7b7cf055c7a9ead992c8961ece7fc27e7906d742a0a7bdfc033`  
		Last Modified: Thu, 15 Apr 2021 02:17:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034a8b17f8de9beb0c46cb63259e8248a28ebd6e0bc538f8f2f28c21b07e98ac`  
		Last Modified: Thu, 15 Apr 2021 02:17:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eadc586391f282b3ba07eaccd595991f7eb491c9945ae266f898f64dcaf2e26`  
		Last Modified: Fri, 07 May 2021 21:17:59 GMT  
		Size: 10.8 MB (10783740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99af69ffc38d32898a3ed370715a7dd54a989bdd01c260b4764c78a4f89a1117`  
		Last Modified: Fri, 07 May 2021 21:17:56 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcefb45687eae751f7189c21b9478b4aec1c3801e490bc5cbeed1b438956d73`  
		Last Modified: Fri, 07 May 2021 21:17:59 GMT  
		Size: 15.0 MB (14974326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4f5cda24024ba577a3b108c7bc2f0b530a7edb2dc847f31dd18cc92d1a6e9`  
		Last Modified: Fri, 07 May 2021 21:17:56 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1674b7182b3df65148f2b7759bc5810c476158280c1ba76f2929e0ed9d5582`  
		Last Modified: Fri, 07 May 2021 21:17:56 GMT  
		Size: 16.9 KB (16872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b96ea2009920239020b5da22d58f0bfa35fd10420db0054a5d8d34b51411178`  
		Last Modified: Fri, 07 May 2021 21:17:56 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac491aa34dc2ba5066cdc52878e3b36642e99e59749d50eaad07b516a2248b`  
		Last Modified: Fri, 07 May 2021 21:44:49 GMT  
		Size: 3.2 MB (3225086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b95736673194bebe97bd85227deef043f8e55027c09c01442630d1832c48d6`  
		Last Modified: Fri, 07 May 2021 21:44:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdf7034f13157c706e29362a45475551a6cfac3dbabee3c146e4d03270b4ef`  
		Last Modified: Fri, 07 May 2021 21:44:48 GMT  
		Size: 553.6 KB (553617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f3e30e0058735d33ecdc6ec319f9bf097a0f4419e1fe38c3e0a9cf7ba39e42`  
		Last Modified: Fri, 07 May 2021 21:44:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513b39c93d6ad1ccad63d09a2e8dc7a11766a0bbf26efcbf99cc83c3eca0a031`  
		Last Modified: Fri, 07 May 2021 21:44:53 GMT  
		Size: 18.9 MB (18862544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; arm variant v6

```console
$ docker pull drupal@sha256:bff7c7e0cd0d87a1e9cd3cd1b9ee8fb8e9d275070775d917992ae6c783dfdfb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50608720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf4b7f17e1f139b0067fe2a8f126010cb6b61b6463436529cf5dcd66fb5f778`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:17:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:17:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:18:02 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:18:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:18:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:23:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 01:23:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:23:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:23:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:23:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 20:21:45 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 20:21:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 20:21:46 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 20:21:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 20:21:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 20:25:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 20:25:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 20:25:50 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 20:25:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 20:25:52 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 20:25:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 20:25:56 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 20:25:57 GMT
EXPOSE 9000
# Fri, 07 May 2021 20:25:57 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 20:49:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 20:49:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 20:49:24 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 20:49:28 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 20:49:30 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 20:50:10 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 20:50:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8cad8c4578c5270a90a55846773ce40754729c5f975e7d1654c5027577be4d`  
		Last Modified: Thu, 15 Apr 2021 02:34:49 GMT  
		Size: 1.3 MB (1332677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95839444ef1cef22cc3ad52750fe13ff8a0a9885523f2a8b0c3cd24f4e484f9`  
		Last Modified: Thu, 15 Apr 2021 02:34:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120021bdf73e23b723057a459e2f4f7bb982a0838bb0cb77140d7b8537d5c154`  
		Last Modified: Thu, 15 Apr 2021 02:34:48 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7eed2cd776db3332d5b088a754a92df4870d004c924900a3083fbe86667cd7`  
		Last Modified: Fri, 07 May 2021 20:29:17 GMT  
		Size: 10.8 MB (10783756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047ae0854bd40b96d74bf96843d03b988db8992dbf673fe61c514587e26cc25a`  
		Last Modified: Fri, 07 May 2021 20:29:15 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481959f3062b32043cc5c3cce4803b298725058428569bdd7f4dd85a3cb7271b`  
		Last Modified: Fri, 07 May 2021 20:29:19 GMT  
		Size: 13.7 MB (13651265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77f5781e312df8422227223b075bb1e33a062250cdaf1efe1c5f863d2393b6a`  
		Last Modified: Fri, 07 May 2021 20:29:14 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcee0dc704556a3d55b2fb1d0505eb7f98ab84232bd6c15dd07a36e23732629`  
		Last Modified: Fri, 07 May 2021 20:29:14 GMT  
		Size: 16.9 KB (16879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa771ada3f727d0dd3c0504bca9f4bad71ed65acb811a3bc50a1af5ea9ffdc9c`  
		Last Modified: Fri, 07 May 2021 20:29:14 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f9fa455f1cbf63ff4a59d376432104f1bb7acc12a55df51ad59691c40dd78f`  
		Last Modified: Fri, 07 May 2021 20:51:41 GMT  
		Size: 2.8 MB (2789167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341355d03861003d28a7b9bdf864b936eb9fce9d0117e7d26db1ce8473e07fbc`  
		Last Modified: Fri, 07 May 2021 20:51:40 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb477533ffb30ffefcbaa568ef42aaf60cd10370982c5262209ce348ba1faaa0`  
		Last Modified: Fri, 07 May 2021 20:51:40 GMT  
		Size: 553.6 KB (553601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f293c77ae7dfafe843999edb0d9cb29725910e75d30aaa0515e3a08844677a`  
		Last Modified: Fri, 07 May 2021 20:51:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90806e19530f0027ead3834ca4289a7a0d0b18eeb66b31afaa7002c6c571309`  
		Last Modified: Fri, 07 May 2021 20:51:52 GMT  
		Size: 18.9 MB (18862782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; arm variant v7

```console
$ docker pull drupal@sha256:a9e48e9b665ea226717c1ec076b6da7296cb993e190590d4ee2c9957565a96a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49199387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0194a999c2fad714c623c387577f3bf4169e94910fa1b4dcd0c887db7e16842a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:20:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:21:07 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:21:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:21:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:22:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:29:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 02:29:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:29:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:29:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:29:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 21:08:02 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 21:08:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 21:08:04 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 21:08:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 21:08:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 21:10:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 21:10:57 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 21:11:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 21:11:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 21:11:02 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 21:11:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 21:11:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 21:11:05 GMT
EXPOSE 9000
# Fri, 07 May 2021 21:11:06 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 22:16:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 22:16:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 22:16:44 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 22:16:45 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 22:16:46 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 22:17:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 22:17:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4e41df07c72800bc526ed5085dfb56b791a44201a4aeb443f6c5cde89b7d2`  
		Last Modified: Thu, 15 Apr 2021 03:40:15 GMT  
		Size: 1.2 MB (1233448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e065d0af38976f008e1bbbfcac343cd709823a229184ee5b77f41b3b5b8cc0a`  
		Last Modified: Thu, 15 Apr 2021 03:40:14 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff291ee936c5a1a0de1ecba3948d82473925b62b72ef884cf505c01ece3ee207`  
		Last Modified: Thu, 15 Apr 2021 03:40:15 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a530e1b8659101f4d4a36d6302d99a246b24bf56f4487e057ec07d1626ab43`  
		Last Modified: Fri, 07 May 2021 21:18:09 GMT  
		Size: 10.8 MB (10783748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0863cda3a81c72dc6c0c1c898c43f24d5727847daff3b79a1221fb1bb8c64e2`  
		Last Modified: Fri, 07 May 2021 21:18:06 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8030f47a7883d3b19cf11c9d512fcd315a3dee7512d4c974cf44961ab09347`  
		Last Modified: Fri, 07 May 2021 21:18:11 GMT  
		Size: 12.8 MB (12798627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ae2a8d6e13f4e8d4550c32372bae4d8e5bc21f0ef72f09d989ee8d9a892d6b`  
		Last Modified: Fri, 07 May 2021 21:18:07 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de75eadcc3eef382550c9e99ff9fda00803bdd245e73fd9efca980d488cf5952`  
		Last Modified: Fri, 07 May 2021 21:18:07 GMT  
		Size: 16.9 KB (16870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41212efe995c259e6802279a43ede212ff7277ff5903aea9987c4bb01968f6fd`  
		Last Modified: Fri, 07 May 2021 21:18:07 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b827b1fcff63a05cfcd08fe850a898a0697c0e456612964726874bc9885960`  
		Last Modified: Fri, 07 May 2021 22:22:16 GMT  
		Size: 2.5 MB (2527859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedeeac290a7052b20bd9fbd096ec4772e71adb607001f28bddc4c066a2235ed`  
		Last Modified: Fri, 07 May 2021 22:22:16 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89046ac36807b6bc7dac2f06fb754ece4070bb69f878d39e24b111b3c3b8c018`  
		Last Modified: Fri, 07 May 2021 22:22:16 GMT  
		Size: 553.6 KB (553612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a56609571f1736abb3b3f54305e5ba68b1a4d9e71a987e79e98b0fb5ea307a2`  
		Last Modified: Fri, 07 May 2021 22:22:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671e88ff98c59b2a80d9bd4c922fcc426dd8dc021ddb3d547f90ee8268be0877`  
		Last Modified: Fri, 07 May 2021 22:22:28 GMT  
		Size: 18.9 MB (18862709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:bea991f0c66fc3d0e42b005c4a6367b525b9e428bde366db3883fbded330665a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51679678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfdc382319425c70d62c8907ff67e2f0f9ee64ed02323f32defdf7a1cf68d86e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:40:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:40:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:40:25 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:40:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:40:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:46:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:46:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:46:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:46:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:46:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 20:17:54 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 20:17:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 20:17:59 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 20:18:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 20:18:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 20:22:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 20:22:05 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 20:22:10 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 20:22:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 20:22:12 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 20:22:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 20:22:16 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 20:22:17 GMT
EXPOSE 9000
# Fri, 07 May 2021 20:22:19 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 20:54:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 20:55:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 20:55:10 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 20:55:12 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 20:55:13 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 20:55:51 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 20:55:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75454ef1d96df8081b852e85f0c79167a62d10ee23634b86540a521a9262b3ad`  
		Last Modified: Thu, 15 Apr 2021 02:00:46 GMT  
		Size: 1.4 MB (1371474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079a2c7ac37c396fe3f4a33ac65c7df4b7d75c46cc1af7f6b4a6f8c37b780d3`  
		Last Modified: Thu, 15 Apr 2021 02:00:45 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f873453c05b9b2d26344f14143ca10c58c99fb398ebc906016e20ed8b9d20b8`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fb82b27904f5ea4b5df2226a1452bdf6dccf06ddc62c070872c6829835e81a`  
		Last Modified: Fri, 07 May 2021 20:29:23 GMT  
		Size: 10.8 MB (10783739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2495fe8349e3cb2f6cfc8e7b62c289f8b2a09e4fe3ed2bf7452253d562e74e`  
		Last Modified: Fri, 07 May 2021 20:29:21 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d5ed36d07f16e9caf0d54e09442b7a2233eaa080c35b067f54c3767f36e2bb`  
		Last Modified: Fri, 07 May 2021 20:29:25 GMT  
		Size: 14.4 MB (14444618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b962831035aa9cf07b040d5211495292f6a8fbdaf288b9e76be424f95d6781b2`  
		Last Modified: Fri, 07 May 2021 20:29:21 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abda7cc310873069f31a5adb903aca4e175e02eba54a376c17a9973aadbe2eb`  
		Last Modified: Fri, 07 May 2021 20:29:21 GMT  
		Size: 16.9 KB (16877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b397cfc9b054d373068a0a8719d19538337973542d348c85bc6a3ba0f20efb5`  
		Last Modified: Fri, 07 May 2021 20:29:21 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a07e7f62754c345062e6781cc1531b2d0f9baffcf88271e7e6a79d6e97dfc14`  
		Last Modified: Fri, 07 May 2021 21:00:52 GMT  
		Size: 2.9 MB (2922511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381979bec5a50ca970a221b4bf026200860620e403e7cbb46921e3d9c2f392a8`  
		Last Modified: Fri, 07 May 2021 21:00:52 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795770910680a4bad4fd42b3205d23f8d255ad727bac6ea2f4ddd73ed24cea15`  
		Last Modified: Fri, 07 May 2021 21:00:52 GMT  
		Size: 553.6 KB (553616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd6c752aba0b9c698e56627253b2e0d45a04aaeadcd17a68440bd48307cb29`  
		Last Modified: Fri, 07 May 2021 21:00:51 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4350a22b1bada8f74bce6485e7fb0c6af0ba55a203d00e564cb05e24e3686`  
		Last Modified: Fri, 07 May 2021 21:01:02 GMT  
		Size: 18.9 MB (18862818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; 386

```console
$ docker pull drupal@sha256:38289d7395152aecd858b39041c89d91e2e614aaa162069fcf2fa513e915c926
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52602138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7569d7ec18d911b28e0fe8141fe58d0a49e268c08e9ee2024f1af71d6c97a774`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:56:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:56:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:57:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:57:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:57:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 04:06:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 04:06:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 04:06:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 04:06:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:06:12 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 20:15:52 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 20:15:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 20:15:53 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 20:15:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 20:15:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 20:20:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 20:20:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 20:20:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 20:20:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 20:20:48 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 20:20:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 20:20:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 20:20:49 GMT
EXPOSE 9000
# Fri, 07 May 2021 20:20:49 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 21:11:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 21:11:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 21:11:24 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 21:11:25 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 21:11:25 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 21:11:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 21:11:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d185111b3910ef52a6032f8cf2734e74728d4d74ae9701e8cee922617f053d6`  
		Last Modified: Thu, 15 Apr 2021 05:59:32 GMT  
		Size: 1.5 MB (1466925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4756ea99511687987d1d551c5f3f65fe89ac052d4a5cd5f65720d2cb2707cd29`  
		Last Modified: Thu, 15 Apr 2021 05:59:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6fc63b3938406dbd05ca0ed1285af5f845efdea8f44a8eacf959403513bb2a`  
		Last Modified: Thu, 15 Apr 2021 05:59:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d146ad7fd2f703595128b0d21db9a873e3f0bf89b4bbaea41bb958088e444a3`  
		Last Modified: Fri, 07 May 2021 20:39:01 GMT  
		Size: 10.8 MB (10783738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb00833e0d3c76156e2997fac2760e974bc550887ec11df835302b990900a8a`  
		Last Modified: Fri, 07 May 2021 20:38:57 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da74bf4a69322ca69eb91590dba1c8d22c18e12af4a917c81888b9523de529c`  
		Last Modified: Fri, 07 May 2021 20:39:02 GMT  
		Size: 15.0 MB (15022125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83af7922037dce19e39f166ebb7eafaf650c22ed9b6213f05833d874c255df77`  
		Last Modified: Fri, 07 May 2021 20:38:57 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5ad69598674c5d208c29505818b85468308cbba4c0649710da5fd751477985`  
		Last Modified: Fri, 07 May 2021 20:38:57 GMT  
		Size: 16.9 KB (16878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7545d33b3d5bf4ec24cb0e5d5b6d479f1239e77027930036fca31bd6d5189e`  
		Last Modified: Fri, 07 May 2021 20:38:57 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a8b626c0d9be4a8858d991fec883287fe75291b2c45a8756b5b6bded2ea20`  
		Last Modified: Fri, 07 May 2021 21:22:51 GMT  
		Size: 3.1 MB (3087335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59059e4f2a67ab2fdd5bf216dad6d7c4033d7902f70778213269fec21bca8c50`  
		Last Modified: Fri, 07 May 2021 21:22:50 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de072333e21d5b208f8d2817d3341388f770411923243939c257108596af564`  
		Last Modified: Fri, 07 May 2021 21:22:50 GMT  
		Size: 553.6 KB (553610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b50ae465cad46c200a32b57487aef09a124c8753f1620980ca33df8a82c8a3`  
		Last Modified: Fri, 07 May 2021 21:22:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873e4bb1f88cce3b7347854e086830a0a0fb96ff426daf74b51f9af910df809d`  
		Last Modified: Fri, 07 May 2021 21:23:02 GMT  
		Size: 18.9 MB (18862397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; ppc64le

```console
$ docker pull drupal@sha256:578a2346d84956a774eb64f9f6d7707a9bb167767d299b9685289e012c77bc7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53178378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444e4ae0933cb2144f62414ae8cdd67efbcd8c9f67256dcac601c38c4974e51d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:32:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:32:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:32:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:32:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:32:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:38:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 20:39:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:39:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:39:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:39:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 21:33:48 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 21:33:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 21:34:10 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 21:34:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 21:34:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 21:38:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 21:38:44 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 21:38:57 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 21:39:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 21:39:17 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 21:39:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 21:40:03 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 21:40:18 GMT
EXPOSE 9000
# Fri, 07 May 2021 21:40:31 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 22:34:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 22:34:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 22:34:40 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 22:34:50 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 22:35:05 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 22:35:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 22:35:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d21396f5076961d8b40ffe92797fa964e2f354badb992076ec2e8c341face0`  
		Last Modified: Wed, 14 Apr 2021 22:02:22 GMT  
		Size: 1.4 MB (1409857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d81f1a419911a96a9173df743dcaa56618dc4f880e30a2d57b6571cd744410`  
		Last Modified: Wed, 14 Apr 2021 22:02:21 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30aa25148a768989691435c0455a034cef0f452dba09512d908f008456da8cb`  
		Last Modified: Wed, 14 Apr 2021 22:02:21 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ee1d55c6183cde93fc78c7484b59245935ae9345a3ea748f4524ee4c6db987`  
		Last Modified: Fri, 07 May 2021 21:51:49 GMT  
		Size: 10.8 MB (10783761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aac28702c45147db49f0d6c07fc0dd4558d423593d3a508229f59d08f59dad5`  
		Last Modified: Fri, 07 May 2021 21:51:44 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f72ea8b94d4e55c8d996930686502686abc8d1617f26423a847b1916084c33`  
		Last Modified: Fri, 07 May 2021 21:51:48 GMT  
		Size: 15.7 MB (15660524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33aebac529f9bd17bf91b73561ab64611e31f3484ae01388a3eb30faed0c10f`  
		Last Modified: Fri, 07 May 2021 21:51:44 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1a401653da50460215f0441c1a907cdf75c0635a6e840dbc1f80ba1bc3b0f6`  
		Last Modified: Fri, 07 May 2021 21:51:44 GMT  
		Size: 16.9 KB (16922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dc12ee73a66b5ecefa4776d24af140ba3fa4bac210c43069966fa13eac280a`  
		Last Modified: Fri, 07 May 2021 21:51:44 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67998b7e01573d46829f5f0cd83dd35bde55e0459fafee9bfc8ae25af444f102`  
		Last Modified: Fri, 07 May 2021 22:45:35 GMT  
		Size: 3.1 MB (3071265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366d33a568a50d4bd3532812746898499b995d965982529eff6a35e0e38a31fb`  
		Last Modified: Fri, 07 May 2021 22:45:34 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6a2a6784f290ed07e54c2085cfcb728dfeac956936f70fd18642b2ae5c17e5`  
		Last Modified: Fri, 07 May 2021 22:45:34 GMT  
		Size: 553.6 KB (553603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0678fde423eac10a4ae2fdbc5896493682bd0962198612fb956655322906c6`  
		Last Modified: Fri, 07 May 2021 22:45:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba34918211bb646a0624e8587dd7076d7d6bafb8a1e9cf1088f46c8a898143`  
		Last Modified: Fri, 07 May 2021 22:45:40 GMT  
		Size: 18.9 MB (18862356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine` - linux; s390x

```console
$ docker pull drupal@sha256:109c552739f4afac983ec94cf8db1790be7e6424479e141ef30fdbd8533df010
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51306790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24ebcbedec4e9efd88daacdc8179192bed9bf3785b7872139af8f3e43f3dca3a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:11:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:11:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:11:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:11:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:11:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:14:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 19:14:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:14:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:14:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:14:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 07 May 2021 20:21:43 GMT
ENV PHP_VERSION=8.0.6
# Fri, 07 May 2021 20:21:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc
# Fri, 07 May 2021 20:21:45 GMT
ENV PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20
# Fri, 07 May 2021 20:21:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 May 2021 20:21:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 May 2021 20:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 May 2021 20:26:53 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 07 May 2021 20:26:55 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 May 2021 20:26:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 May 2021 20:26:56 GMT
WORKDIR /var/www/html
# Fri, 07 May 2021 20:26:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 May 2021 20:26:58 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 May 2021 20:26:59 GMT
EXPOSE 9000
# Fri, 07 May 2021 20:27:00 GMT
CMD ["php-fpm"]
# Fri, 07 May 2021 21:03:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 May 2021 21:03:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 May 2021 21:03:47 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Fri, 07 May 2021 21:03:48 GMT
ENV DRUPAL_VERSION=9.1.8
# Fri, 07 May 2021 21:03:48 GMT
WORKDIR /opt/drupal
# Fri, 07 May 2021 21:04:11 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 May 2021 21:04:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c20a3ecae8cc7ea51ca293c87d17bf04cefeb04d12ffb9652a9766be3f8416`  
		Last Modified: Wed, 14 Apr 2021 20:02:02 GMT  
		Size: 1.4 MB (1382747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc1d01c306c098f90edda1998ec952dd13e38675b3fed5e7b73efb281d45223`  
		Last Modified: Wed, 14 Apr 2021 20:02:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d0bbd337de43d24bc0a30a3e902ab2dc6a3a37d4c24d543cf4b39987ecb649`  
		Last Modified: Wed, 14 Apr 2021 20:02:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51bed2680b59af41145a07543400e2e13908de0dd45708970835a2466f7b91`  
		Last Modified: Fri, 07 May 2021 20:33:29 GMT  
		Size: 10.8 MB (10783749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e93c287195546a86dbda393a2c1375b59b77538231e556d3d23008e1336ff`  
		Last Modified: Fri, 07 May 2021 20:33:27 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3444726b9f84d96a191d1652ac3d9a45b7ee3351fc0cc4fb03bb8379d168ed33`  
		Last Modified: Fri, 07 May 2021 20:33:29 GMT  
		Size: 14.2 MB (14188233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf14907fbbf64107cc80de8018a782032b1c41766ce4ef59c47d794b60f7c16`  
		Last Modified: Fri, 07 May 2021 20:33:27 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28eba180cb77059793bd0bb5c95dedaf1868a6cd42c012444d3337bce563f8f`  
		Last Modified: Fri, 07 May 2021 20:33:26 GMT  
		Size: 16.9 KB (16914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4df29eece765ddec89277088f9437d4b250c8164911e3ef8adcf56255c01ec`  
		Last Modified: Fri, 07 May 2021 20:33:27 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6022fad6905f22b71bc59455d3a623a3cad335995d545ad0e81c0082100f3bea`  
		Last Modified: Fri, 07 May 2021 21:09:19 GMT  
		Size: 2.9 MB (2937240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4f96c3ae18f7f7f7eebb0f167a38cb74f61a3958d422aa63988865a59e6530`  
		Last Modified: Fri, 07 May 2021 21:09:19 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2472afb60ee906faea3461cc6bcb0980346e73085144aa09c69ce776e7bcd2c`  
		Last Modified: Fri, 07 May 2021 21:09:19 GMT  
		Size: 553.6 KB (553611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3719f9b467b9a8f35488b3dbe575ddcd927690a0b7d0d570fa8af5a7f35aa6`  
		Last Modified: Fri, 07 May 2021 21:09:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12a3ef57f01715fd08496981c82930bf353382a2fd327fa6c4a53f0600c481d`  
		Last Modified: Fri, 07 May 2021 21:09:23 GMT  
		Size: 18.9 MB (18862529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
