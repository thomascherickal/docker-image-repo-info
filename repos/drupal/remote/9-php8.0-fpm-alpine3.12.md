## `drupal:9-php8.0-fpm-alpine3.12`

```console
$ docker pull drupal@sha256:93eb574ea6ac975590021450196b1d456147d3fb562132c69b329c15ebd2cf59
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

### `drupal:9-php8.0-fpm-alpine3.12` - linux; amd64

```console
$ docker pull drupal@sha256:87831c772510edbe9b9a701d627c2398662f9cf7886db5fd5a8fc1d4a2027639
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52500874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a275a426afa3cb53655d6291d183c1b388534a405ee1f9d9f5672fcaafc5c50`
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
# Thu, 29 Apr 2021 18:29:06 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:29:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:29:07 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:29:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:29:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:37:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:37:13 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:37:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:37:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:37:16 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:37:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:37:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:37:19 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:37:19 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 21:11:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 21:11:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 21:11:33 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 20:20:15 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 20:20:16 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 20:20:25 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 20:20:26 GMT
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
	-	`sha256:dfd4a6e3e1ea9524d772a36a287508fdbe30a7a5ea98c440475002d2125596e8`  
		Last Modified: Thu, 29 Apr 2021 20:19:45 GMT  
		Size: 10.7 MB (10685281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49738e60c04bcbd0202882edcb6e1059fdd78127e399fb6cc98077eea109390`  
		Last Modified: Thu, 29 Apr 2021 20:19:41 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4716dbb7c7365772dc96e08c7a40a5199d59f6e7439db7413ebb8ba375ac855b`  
		Last Modified: Thu, 29 Apr 2021 20:19:44 GMT  
		Size: 15.0 MB (14974539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7298ebfb2a9fc6d4b5f6d1f5389669cdef5ca64d7fcf043969aa9fe6d223e5`  
		Last Modified: Thu, 29 Apr 2021 20:19:41 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f88eb88192c71cae42752b23f19850069a022e17eabbaf6afae03ff1255cc04`  
		Last Modified: Thu, 29 Apr 2021 20:19:41 GMT  
		Size: 16.9 KB (16878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5626128f13aab24adfe62dd01a018ab7efdd61f33c426aca1e750c4c1325e7bd`  
		Last Modified: Thu, 29 Apr 2021 20:19:41 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824d4bfd3ba74ed62dc5f2ecafef6727ce14424466c7aad1e521e1e96503036f`  
		Last Modified: Thu, 29 Apr 2021 21:18:07 GMT  
		Size: 3.2 MB (3225131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd24d3dc55c4373f002051644aa043f5916a9fe1a8271e185e3261d9c2a05be`  
		Last Modified: Thu, 29 Apr 2021 21:18:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478d980d86d2213ceae355835a9f70d5ed1b4fa236a90869184c1c947ac04a47`  
		Last Modified: Thu, 29 Apr 2021 21:18:06 GMT  
		Size: 553.6 KB (553615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544ac35cc353526fccb52362e383d61a4258277ffde426462ca41c2be906e617`  
		Last Modified: Wed, 05 May 2021 20:30:43 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6c2848977a6f32df2cbffb5af9d9070f5cda0aa4ace8c9ae7b82b30c7d6216`  
		Last Modified: Wed, 05 May 2021 20:30:48 GMT  
		Size: 18.9 MB (18862331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; arm variant v6

```console
$ docker pull drupal@sha256:50ea680f91bdd7670978ea5ad4e7b9f6ca5ae0dea62ef246f1708d1bbe569e8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50510464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f799e421959279f406f5fc84e5eaadc336e14baae9e6539d31c83e8bf6c90138`
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
# Thu, 29 Apr 2021 18:28:43 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:28:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:28:46 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:28:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:28:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:32:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:32:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:32:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:32:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:32:55 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:32:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:33:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:33:05 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:33:08 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 19:26:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 19:26:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 19:26:42 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 19:49:36 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 19:49:37 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 19:50:06 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 19:50:13 GMT
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
	-	`sha256:f7f8703c5828050a380a2ea88a2b71594d8cf45cddb307e961a9556320365315`  
		Last Modified: Thu, 29 Apr 2021 19:03:05 GMT  
		Size: 10.7 MB (10685295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41706b5ae573645888e3118e366999acf2a5e6885b9f038dc91bfbbe6188884f`  
		Last Modified: Thu, 29 Apr 2021 19:03:02 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f742d12d333aaa21f9e906b762f02dea229a03496e76f3d7e541cda879c09cbc`  
		Last Modified: Thu, 29 Apr 2021 19:03:08 GMT  
		Size: 13.7 MB (13651421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad4e565f08673b1b53489ac4c392e8408970ccbee59ca4f5042a2a5b86bfbfe`  
		Last Modified: Thu, 29 Apr 2021 19:03:02 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb75b7578a8183ed48ed403461cb20ec168a508890f03f195d7a37d46d98f8e8`  
		Last Modified: Thu, 29 Apr 2021 19:03:02 GMT  
		Size: 16.9 KB (16883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036599586250e26203c45739c4e997d7af3db5d976b7c0fcac73e611b9cfbc79`  
		Last Modified: Thu, 29 Apr 2021 19:03:02 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39797d650112cfe8e37939f84c49c0a6674d60623016029b8f39c8715a4d3d66`  
		Last Modified: Thu, 29 Apr 2021 19:28:35 GMT  
		Size: 2.8 MB (2789203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a509c95187c9bef474681ec0f61e261005b433b1837cf6fd3f126785cf9b7eb8`  
		Last Modified: Thu, 29 Apr 2021 19:28:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9833921a00f7f0e9fe42d03b7da20cabb3e0b1e815afcc0e99be4288f85dfa`  
		Last Modified: Thu, 29 Apr 2021 19:28:34 GMT  
		Size: 553.6 KB (553610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea5ebc3d06723fa435614b57f21da64a5fb7d7905571c6c3c688f195c723032`  
		Last Modified: Wed, 05 May 2021 19:54:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c254fde4e410edb4c04211361575eb264985c2146cb326c01ba5872177df27ae`  
		Last Modified: Wed, 05 May 2021 19:55:06 GMT  
		Size: 18.9 MB (18862777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; arm variant v7

```console
$ docker pull drupal@sha256:abb50ae88e16c29375db3c4a97e0ed35165f8d02660433de10ec1a28ce7ab39b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49101166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11fa28353307cae22fef8e4f40a5437c35b231f0c8fa0a744e3b038ddc6157ee`
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
# Thu, 29 Apr 2021 18:32:43 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:32:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:32:46 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:32:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:32:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:36:02 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:36:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:36:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:36:12 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:36:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:36:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:36:18 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:36:18 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 20:44:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 20:44:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 20:44:35 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 20:02:38 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 20:02:42 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 20:03:32 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 20:03:42 GMT
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
	-	`sha256:1fdc36b305cfb23ae8eadde2353b5c3f7d6ac647d207e7eb6754e36a4f46376d`  
		Last Modified: Thu, 29 Apr 2021 19:39:44 GMT  
		Size: 10.7 MB (10685278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcd1c16e9f96e5f4d17b2f62560a02ec013a6c460d984d762d7e7fa714a6fee`  
		Last Modified: Thu, 29 Apr 2021 19:39:41 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cba9f9d41c88bb4268790d4c1c2452ccaf0cd2876900c16b359a27b225c9a43`  
		Last Modified: Thu, 29 Apr 2021 19:39:47 GMT  
		Size: 12.8 MB (12798660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299bc93d5ce2009bc66f6e0e4b2ea4b94825293ea48e0db445ff5e67dfd11993`  
		Last Modified: Thu, 29 Apr 2021 19:39:41 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4904b8c50334d79f0f978df4c17a055e62df84497659309c2a7c3dfc861867fd`  
		Last Modified: Thu, 29 Apr 2021 19:39:41 GMT  
		Size: 16.9 KB (16875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2856eac50001f171a55a455f1b0d58ffc33408d6b1517cf57b2c2a2d58d3e40`  
		Last Modified: Thu, 29 Apr 2021 19:39:41 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1c0411dbb662e5da3e0d3a43c0e46b6bfd80ab27f8bec0932cda313c3dc6d`  
		Last Modified: Thu, 29 Apr 2021 20:51:13 GMT  
		Size: 2.5 MB (2527896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48cbde8be33cd3f6579a96ade3e7b28cf9b466487dd012270b6f459bd41a29`  
		Last Modified: Thu, 29 Apr 2021 20:51:12 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea4ea0ab6da9ea9956b5b7c4fb8ba6fb9d2d572be8e59457a7f551b24eeee3f`  
		Last Modified: Thu, 29 Apr 2021 20:51:12 GMT  
		Size: 553.6 KB (553611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3ea9753ca2f5e56eb72b177e763ff9ae7b3917c6cb35b7c7e6c8ffc688b8a7`  
		Last Modified: Wed, 05 May 2021 20:25:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976ddf120c2f4f55f3ebdc1d308c3db7df3ac4102b03dd8fc5387f9355f7aa7`  
		Last Modified: Wed, 05 May 2021 20:26:33 GMT  
		Size: 18.9 MB (18862885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:b77bf421adfec2e8d176164c9d27d57a35b73865dd82f34be2742f14a8cf6549
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51581374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bb6930098f78d9c932c035ee9e3f74284b3fa584409ac1687e3ca725ab2cb8b`
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
# Thu, 29 Apr 2021 18:34:40 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:34:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:34:43 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:34:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:34:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:38:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:38:40 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:38:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:38:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:38:49 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:38:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:38:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:38:55 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:38:56 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 20:26:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 20:26:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 20:26:14 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 19:41:22 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 19:41:23 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 19:41:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 19:41:47 GMT
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
	-	`sha256:d5a3f4850f6024db498e1bd0dcbf40c33b17a41cbad7c88304ba04569eb672a7`  
		Last Modified: Thu, 29 Apr 2021 19:47:11 GMT  
		Size: 10.7 MB (10685280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8438d10aee9e902a506ebcc7fbe433b2de145c2a95cde5cfc05687cf99010ef6`  
		Last Modified: Thu, 29 Apr 2021 19:47:08 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e46f67c0f24baf269ca314ebb1b898175d716c2a3b4df83aae0b73a7cb739f`  
		Last Modified: Thu, 29 Apr 2021 19:47:12 GMT  
		Size: 14.4 MB (14444627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959bed2cc39401b575832f87f999ea25c82526a4f692bd002dc37745c7309520`  
		Last Modified: Thu, 29 Apr 2021 19:47:08 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f99e943b169ced80ba0be3a4a091c985daa56585761ba366d495d80ed7a0`  
		Last Modified: Thu, 29 Apr 2021 19:47:08 GMT  
		Size: 16.9 KB (16879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd21f30d36c44c2571cbba115ab9dfa2d669748a5e3c20e2f8cbead4b56a5b6`  
		Last Modified: Thu, 29 Apr 2021 19:47:08 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e304e92f7aed63f69349d47986b070b91fea251d814ce9a74c83ad08b722fd`  
		Last Modified: Thu, 29 Apr 2021 20:33:27 GMT  
		Size: 2.9 MB (2922625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3bdff2fe0aa351f08f856b57f01e9c0cb5e05bec362ec24cda467f39274bc`  
		Last Modified: Thu, 29 Apr 2021 20:33:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3695fe6daad1900f18e2f3135e38077b150ce0735a440c880d63aa89d552d6b`  
		Last Modified: Thu, 29 Apr 2021 20:33:26 GMT  
		Size: 553.6 KB (553615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091868efc6beb4a7015c43d96e802d72403039478bc958a04543c066f4890adb`  
		Last Modified: Wed, 05 May 2021 19:53:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5746f41d2c1ab0128ee0245a94edc27b727197bd9fb5d8dd24965e901d779c01`  
		Last Modified: Wed, 05 May 2021 19:53:21 GMT  
		Size: 18.9 MB (18862845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; 386

```console
$ docker pull drupal@sha256:4939ec20670a2da94723d934158da171b948e57e882dfabe0cf84409437c6140
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52503704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b9482859894c6528149dca21bd8bbe11487ca21b7c66d28785f589156465eb9`
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
# Thu, 29 Apr 2021 18:41:31 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:41:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:41:31 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:41:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:41:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:48:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:48:23 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:48:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:48:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:48:24 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:48:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:48:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:48:26 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:48:26 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 21:25:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 21:25:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 21:25:42 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 19:39:44 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 19:39:44 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 19:39:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 19:39:56 GMT
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
	-	`sha256:49f9f6ea0157b8d14ad0c60589baf5e5931dbaf3509907e7333d29af7570276e`  
		Last Modified: Thu, 29 Apr 2021 20:37:45 GMT  
		Size: 10.7 MB (10685281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4040726dce1c459e2b9917a01a5e5eba3542c8aa63def07fdc7039bdadda78d2`  
		Last Modified: Thu, 29 Apr 2021 20:37:41 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a77d2616cda61ae2cc8b95e0978f4da5f83a97465a63f8ca75679c4b3dd828`  
		Last Modified: Thu, 29 Apr 2021 20:37:45 GMT  
		Size: 15.0 MB (15022088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2f2d95eb8f17e92f2218e3ee1ba9ffdc146a60d15a54a763fee51b9b2781fb`  
		Last Modified: Thu, 29 Apr 2021 20:37:41 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aad750ea8f55cf7650690b6ec801b3440d5c8aff233dbe025fad6437440dee`  
		Last Modified: Thu, 29 Apr 2021 20:37:41 GMT  
		Size: 16.9 KB (16880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb79b7ff593df2e24d06f72321870a55884ef37c9252314e1673967c20da47`  
		Last Modified: Thu, 29 Apr 2021 20:37:41 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056461172a3dbad4205b5f47e7ce5b70a1ba2c47e9232cdc18d268ae8e959112`  
		Last Modified: Thu, 29 Apr 2021 21:37:33 GMT  
		Size: 3.1 MB (3087394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4851bf85048eddf587d174e8ca6d501fdcc26f75c450e91176f9fd803ddcf54`  
		Last Modified: Thu, 29 Apr 2021 21:37:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3818525a8883c440f14a80f93eadb55ea4a8f721cf61101748570d0b0607aa5`  
		Last Modified: Thu, 29 Apr 2021 21:37:32 GMT  
		Size: 553.6 KB (553613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041a9c918b41a146fd92a8659a67330ca6604dbfd69cbe616f1a791227d6afa9`  
		Last Modified: Wed, 05 May 2021 19:55:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c930335afa1e4618d9c47313ffcc09f090ebfda1336a69d9cd3a53b08e572c42`  
		Last Modified: Wed, 05 May 2021 19:55:28 GMT  
		Size: 18.9 MB (18862392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; ppc64le

```console
$ docker pull drupal@sha256:24ef640ab730184c21e9f7ee8beb0f22de809da4f1181bb41a96e07bfc2071d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53080078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317e9b6366e93181d7722961cdf76f2915fe7894575327d14827a16b81ff3c7d`
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
# Thu, 29 Apr 2021 18:45:42 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:45:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:45:53 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:46:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:46:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:51:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:51:07 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:51:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:51:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:51:39 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:52:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:52:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:52:24 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:52:38 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 20:59:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 20:59:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 20:59:37 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 20:23:43 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 20:23:52 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 20:25:02 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 20:25:24 GMT
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
	-	`sha256:d3cef0c0f86d2770a7b1aedb01abd338c17e6fe6720f003a12a6134148385efd`  
		Last Modified: Thu, 29 Apr 2021 20:24:42 GMT  
		Size: 10.7 MB (10685295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9192c15081c7d05ed0adb806b92304e8a67bbb7759304ceb1f6bde4b5f585ed`  
		Last Modified: Thu, 29 Apr 2021 20:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d18dd5a3568da21946ae27d7327584ed6b673c5942211f6ae1bf6af95fe62c`  
		Last Modified: Thu, 29 Apr 2021 20:24:40 GMT  
		Size: 15.7 MB (15660240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe0ad08359a9f4702eb4e7b0895c2b91f826c17ad23f0af9afc53d80af8bea4`  
		Last Modified: Thu, 29 Apr 2021 20:24:36 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd6d2b75a112c0a05b4a1f1499eb9d7af9c5516d45119f93bbd7ce11c5bebd2`  
		Last Modified: Thu, 29 Apr 2021 20:24:36 GMT  
		Size: 16.9 KB (16921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9177cee0988a909c994e66345b11fa3fec3dd6d181953d2da42ef09343fa6`  
		Last Modified: Thu, 29 Apr 2021 20:24:36 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95eb8ecce1a964c91e36e32b64dec1008804867b9ba143eea4442c61839ae11`  
		Last Modified: Thu, 29 Apr 2021 21:08:53 GMT  
		Size: 3.1 MB (3071352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872b07de597b760f5d0a29be79211ae94a878ffe2fa6615594d65e3ce3e0d1b0`  
		Last Modified: Thu, 29 Apr 2021 21:08:52 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c38e10eb29aa2b0b7689adc52d16baef87a438a650d6cd332a5f65560e16c4`  
		Last Modified: Thu, 29 Apr 2021 21:08:53 GMT  
		Size: 553.6 KB (553610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41ea1024c625040fbd54208fb6337338680a0bc0ece51533e6495d796f8fabe`  
		Last Modified: Wed, 05 May 2021 21:06:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28fc79022a2e87a33764336427f337f2fc199da166ca7dd8d01f93a8cf07980`  
		Last Modified: Wed, 05 May 2021 21:08:42 GMT  
		Size: 18.9 MB (18862714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php8.0-fpm-alpine3.12` - linux; s390x

```console
$ docker pull drupal@sha256:e77eff81359c8e2ef71e3114a0dcf22b451ddab0bf4144c225c813b37259b821
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51208703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2024d3b40e497476f7193cb8a13671e699c285070d8e3a12f226037e3f4e9c`
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
# Thu, 29 Apr 2021 18:13:40 GMT
ENV PHP_VERSION=8.0.5
# Thu, 29 Apr 2021 18:13:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.5.tar.xz.asc
# Thu, 29 Apr 2021 18:13:41 GMT
ENV PHP_SHA256=5dd358b35ecd5890a4f09fb68035a72fe6b45d3ead6999ea95981a107fd1f2ab
# Thu, 29 Apr 2021 18:13:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Apr 2021 18:13:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:16:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Apr 2021 18:16:55 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Apr 2021 18:16:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Apr 2021 18:16:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Apr 2021 18:16:56 GMT
WORKDIR /var/www/html
# Thu, 29 Apr 2021 18:16:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Apr 2021 18:16:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Apr 2021 18:16:58 GMT
EXPOSE 9000
# Thu, 29 Apr 2021 18:16:58 GMT
CMD ["php-fpm"]
# Thu, 29 Apr 2021 19:23:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Apr 2021 19:23:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Apr 2021 19:24:00 GMT
COPY file:20390c476a1bc7f23dc8bedabe5e75de97e68285a5be453cf8394b2a6cacbd09 in /usr/local/bin/ 
# Wed, 05 May 2021 19:43:58 GMT
ENV DRUPAL_VERSION=9.1.8
# Wed, 05 May 2021 19:43:58 GMT
WORKDIR /opt/drupal
# Wed, 05 May 2021 19:44:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 05 May 2021 19:44:40 GMT
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
	-	`sha256:cd1c5afaec2c16baef50b4387f0522853d4a50cd299adaef0ac4c0d72c84d006`  
		Last Modified: Thu, 29 Apr 2021 19:02:32 GMT  
		Size: 10.7 MB (10685287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c632aeaf63750d6c03108af8d324848203232d4afdcf63db3fe0f337d89b1f`  
		Last Modified: Thu, 29 Apr 2021 19:02:29 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b3038cbe00b413164e56d15decc4d1409151648d1412c77e5690726f2cdaec`  
		Last Modified: Thu, 29 Apr 2021 19:02:32 GMT  
		Size: 14.2 MB (14188176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce44d588d5313585826b0f50b19076e7ff34a040e6ba2e5c07a4ba000820065`  
		Last Modified: Thu, 29 Apr 2021 19:02:29 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085f729759cbd7fae4926dda832cf540e97f13cf74ffbda53b39869b5d51103b`  
		Last Modified: Thu, 29 Apr 2021 19:02:29 GMT  
		Size: 16.9 KB (16908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23d77207579fb0bbdf8f6e5aef9078c32fdc4b04a05786face5a17b04b09339`  
		Last Modified: Thu, 29 Apr 2021 19:02:29 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba5e5833254c87297be7299262b1ce7098bb0ee9b7b52fc0a3d28946b402675`  
		Last Modified: Thu, 29 Apr 2021 19:28:22 GMT  
		Size: 2.9 MB (2937322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2828443e75ef3b1170eeb001b05a13f0b09554be337eec86dca84a7dc31b6c11`  
		Last Modified: Thu, 29 Apr 2021 19:28:22 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4cfac35a10a74ebae0b707d8add0915d4193fc0e3249891962e62d120347fc`  
		Last Modified: Thu, 29 Apr 2021 19:28:22 GMT  
		Size: 553.6 KB (553613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f88e81686258ac4a2a4a28e4d30f2c45804690728f1d74dad3a8a39df2a63`  
		Last Modified: Wed, 05 May 2021 20:03:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3528c394aa36c6fe9b6921a4f799f4a406cd265046d7190c3a14f20ebec43615`  
		Last Modified: Wed, 05 May 2021 20:03:21 GMT  
		Size: 18.9 MB (18862890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
