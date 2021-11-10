## `drupal:php8.0-fpm-alpine3.13`

```console
$ docker pull drupal@sha256:e07a403042369853eca9b89a408550f42cccf802851550678936dc438b93fba7
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

### `drupal:php8.0-fpm-alpine3.13` - linux; amd64

```console
$ docker pull drupal@sha256:db8c224257aa0452b1e27b80d521e2b7fcfc9e0699fd59cf428643863cb16670
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52562429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8a138533bd9fad517dcfbea99499ed6505e9a9b91c4f98d27e8bbfe388a423`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 04:00:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 04:00:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 04:00:19 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 04:00:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 04:00:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 04:00:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 04:00:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 04:00:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 04:17:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 16:29:03 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 16:29:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 16:29:03 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 16:29:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 16:29:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:48:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 16:48:12 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:48:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 16:48:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 16:48:15 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 16:48:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 16:48:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 16:48:17 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 16:48:18 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 18:18:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 18:18:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 10 Nov 2021 20:45:04 GMT
COPY file:8534166b12f0b4bb92e85a7bb184cdd5874be64ea494cf9fe702cd43a4a50b79 in /usr/local/bin/ 
# Wed, 10 Nov 2021 20:45:04 GMT
ENV DRUPAL_VERSION=9.2.8
# Wed, 10 Nov 2021 20:45:04 GMT
WORKDIR /opt/drupal
# Wed, 10 Nov 2021 20:45:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 10 Nov 2021 20:45:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f73c0505feff97099f0198262a893c7591884904c0595d39c8825c60506ac`  
		Last Modified: Wed, 01 Sep 2021 05:17:53 GMT  
		Size: 1.7 MB (1707686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d10375732079c31a31aa416c500526f9fea1b9add9764883167734b851a1e8c`  
		Last Modified: Wed, 01 Sep 2021 05:17:52 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d05dc8bbc6681ed10a3260ac9935232133f477566735176bec3f913fec89c1`  
		Last Modified: Wed, 01 Sep 2021 05:17:52 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef81a5c99ec209299c41ddc8bd25c9c8c67e30a2cffc8466188895b3bc16c4d`  
		Last Modified: Thu, 21 Oct 2021 17:01:38 GMT  
		Size: 10.7 MB (10733543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96c9fa53ffbf3056f8f5f13b90ac6a9c9d379d68c934b3694de6e937a66b384`  
		Last Modified: Thu, 21 Oct 2021 17:01:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f1dee20c2020cbcf5a368f6fdc195f90478e910ed400298cde7a8fb8672a75`  
		Last Modified: Thu, 21 Oct 2021 17:02:12 GMT  
		Size: 15.3 MB (15303023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7bae4d25792ae9883d6ac0e6697c23ce488029bb506164495cdc87b2c1399`  
		Last Modified: Thu, 21 Oct 2021 17:02:08 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33347d5da43a8a57fcf77d421e6945a5b33f31b319cb05dfcd08f05656913780`  
		Last Modified: Thu, 21 Oct 2021 17:02:08 GMT  
		Size: 17.6 KB (17633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92ad60685f4cec40e182f4859c561fd25448e48f8430e20a1998e97f600770f`  
		Last Modified: Thu, 21 Oct 2021 17:02:08 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1627b2ea9b8e64b512e9014c250da8b517b0d0a2291be281fa698808a2235359`  
		Last Modified: Thu, 21 Oct 2021 18:33:51 GMT  
		Size: 2.2 MB (2220396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f00a7f28cb89ba9200dd81d593d1c6a40735115fb8e175e799e7321f169636`  
		Last Modified: Thu, 21 Oct 2021 18:33:51 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae8b59c6e5d1eb4bc0884999829a00904fee0d09b02f5184d3c9741e153159`  
		Last Modified: Wed, 10 Nov 2021 20:55:19 GMT  
		Size: 564.1 KB (564137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21504c2623843b253e37966bbe2d65de4d47fd9c5dd4666b6e465115680abd3`  
		Last Modified: Wed, 10 Nov 2021 20:55:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4206d4f3027b79797cc4f20a19801fcf46ddf8deb6f0cdcde2873a561f9898`  
		Last Modified: Wed, 10 Nov 2021 20:55:24 GMT  
		Size: 19.2 MB (19188557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; arm variant v6

```console
$ docker pull drupal@sha256:4374386270bc7783368f6bcac1c91357140ca5d1d63d751add0b6068f15aeb6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50559063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30542ac0049b979fc8ec241acb7121c17d72fe8bc2dcc36f0f1084b11b487c50`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:44:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 05:44:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 05:44:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 05:44:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 05:44:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 05:44:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 05:44:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 05:44:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 05:56:58 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 16:02:14 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 16:02:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 16:02:15 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 16:02:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 16:02:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:12:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 16:12:11 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:12:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 16:12:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 16:12:14 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 16:12:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 16:12:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 16:12:16 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 16:12:17 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 16:54:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 16:54:52 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Nov 2021 21:08:33 GMT
COPY file:80d4bf27c2e7b39ab20a213acb94fe5d80ca22e3a11094d46fda4ad832320763 in /usr/local/bin/ 
# Fri, 05 Nov 2021 00:51:02 GMT
ENV DRUPAL_VERSION=9.2.8
# Fri, 05 Nov 2021 00:51:02 GMT
WORKDIR /opt/drupal
# Fri, 05 Nov 2021 00:51:30 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 05 Nov 2021 00:51:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3fc98133684709161469bcef701e0940a908311477ce7f15df72f49fb2e8cd`  
		Last Modified: Wed, 01 Sep 2021 06:54:28 GMT  
		Size: 1.7 MB (1696436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd64da81d3099d1ab8339d2fa59831a5089160291456bd2c39440133056619f`  
		Last Modified: Wed, 01 Sep 2021 06:54:27 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d585dadec23ae67f4733e9ef2b466376579b31c77c766ca1990da5b51ac8d`  
		Last Modified: Wed, 01 Sep 2021 06:54:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7562bdf647f953849774e209a60fbe0d170246ee61fb7c597043194d25f22d`  
		Last Modified: Thu, 21 Oct 2021 16:25:48 GMT  
		Size: 10.7 MB (10733526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742f26e00f78dd06a106c6b570add9a494d4a5889e2ba73ba1a296d7f43d188d`  
		Last Modified: Thu, 21 Oct 2021 16:25:45 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f168ec5b3612c53c663fe12ed0842752f095b1e9273260de2532f24aadae15d2`  
		Last Modified: Thu, 21 Oct 2021 16:26:46 GMT  
		Size: 13.9 MB (13941516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d794758c50542f60cf73a3535e3c32d35cf1e4ade54fd5712bbe09c6c06daac`  
		Last Modified: Thu, 21 Oct 2021 16:26:35 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9830ffb7779b52d59ab6e5ea44733830afb861f15271173863d79e1ea24725c7`  
		Last Modified: Thu, 21 Oct 2021 16:26:35 GMT  
		Size: 17.6 KB (17622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b3f1917f703b4c6ee25f0037682779023d64d128fd7998e816bdec4c260eec`  
		Last Modified: Thu, 21 Oct 2021 16:26:35 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d7cffa2ddb1ac632888a23d0965b3c7b74c25c8b8fe5bd71fece49ce310c52`  
		Last Modified: Thu, 21 Oct 2021 17:04:51 GMT  
		Size: 1.8 MB (1779993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70805c1c25f2eb2b7fa73d1f27facd7256cf3ad8efe5ef322e911a6f7de2f7d1`  
		Last Modified: Thu, 21 Oct 2021 17:04:51 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754bad132cebcead7ad0b2b0e6603b0f9ae886e4542a1079888a940d852d4ae1`  
		Last Modified: Tue, 02 Nov 2021 21:30:40 GMT  
		Size: 563.7 KB (563748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689f277627376d9d36a1d5a718743643dec52695622d52a010edbaeb4a61304`  
		Last Modified: Fri, 05 Nov 2021 01:01:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad41ea1e811654e58a7d7b32fd4c5591abe45fc24629d330245467030f0dc5a`  
		Last Modified: Fri, 05 Nov 2021 01:01:47 GMT  
		Size: 19.2 MB (19189087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; arm variant v7

```console
$ docker pull drupal@sha256:b029229952711d1a2eb987fbd5c0b99b8ab751dd0240f597691e62b14a3ca753
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49164103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5606e64f7f7f70fff5ae40bb836d984e223e8f5e01893fad7da989a729f8ce51`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Sep 2021 01:26:54 GMT
ADD file:4a3cd5b6e6a9e76edf236ec86eb493ae8b09bf3220a8c0fdcaa474b9d6135ad3 in / 
# Wed, 01 Sep 2021 01:26:55 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 08:33:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 08:33:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 08:33:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 08:33:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 08:33:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 08:33:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 08:33:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 08:33:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 08:45:52 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 17:43:49 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 17:43:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 17:43:50 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 17:44:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 17:44:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 17:52:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 17:52:44 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 17:52:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 17:52:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 17:52:48 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 17:52:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 17:52:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 17:52:50 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 17:52:50 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 21:14:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 21:14:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Nov 2021 22:10:37 GMT
COPY file:80d4bf27c2e7b39ab20a213acb94fe5d80ca22e3a11094d46fda4ad832320763 in /usr/local/bin/ 
# Fri, 05 Nov 2021 03:13:13 GMT
ENV DRUPAL_VERSION=9.2.8
# Fri, 05 Nov 2021 03:13:14 GMT
WORKDIR /opt/drupal
# Fri, 05 Nov 2021 03:13:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 05 Nov 2021 03:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:48fad15491f9799a77d01e4a4a3b0e201ca2aba6f0849c39afa1160d6f3d905a`  
		Last Modified: Wed, 01 Sep 2021 01:28:39 GMT  
		Size: 2.4 MB (2425373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36910c7c08ce3e1586efd7eb24f42e9dada498387dadc80b895a0b3d332b24d`  
		Last Modified: Wed, 01 Sep 2021 09:48:34 GMT  
		Size: 1.6 MB (1564353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929acc3e9f54e70962430426581f4f176551caa52e34e65e93c75472142804c4`  
		Last Modified: Wed, 01 Sep 2021 09:48:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a5fcafd8008c5185f43d58e5532462ce49fd149bea65a2716ba1a9c2522f0b`  
		Last Modified: Wed, 01 Sep 2021 09:48:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18548def28ef59bb873f98cdde68a5f18de92b73cf7a283cbe01e4a64d234065`  
		Last Modified: Thu, 21 Oct 2021 18:27:40 GMT  
		Size: 10.7 MB (10733539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40c641ba6829cd35147f21eca613d62dc6ad51ea970cb33ce97bd1751de1a3c`  
		Last Modified: Thu, 21 Oct 2021 18:27:38 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a47882e9590a8a951278c01ff937b48b9a93d39db32e524cabdeceabc07d90c`  
		Last Modified: Thu, 21 Oct 2021 18:28:33 GMT  
		Size: 13.0 MB (13049086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d71cc5732a6d51ebd43aad134b01eb100828d55c8e8fc97c74045a9a6ca5cd`  
		Last Modified: Thu, 21 Oct 2021 18:28:24 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31dac0344c2dea2e94ff024ad0109020eb8787588c1a246760258062ac2a9b6`  
		Last Modified: Thu, 21 Oct 2021 18:28:23 GMT  
		Size: 17.6 KB (17626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4956c4b737fc30cb0f7370152c440cef32ac07bb5996a586d080275f971656`  
		Last Modified: Thu, 21 Oct 2021 18:28:23 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cb838aae79e0f25adca2365471d9c79ea4daebc4ac8b01ac5c1a5e4033d0e1`  
		Last Modified: Thu, 21 Oct 2021 21:56:13 GMT  
		Size: 1.6 MB (1608368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3319806f22949552882973b5816a16f46b439b636464a47ce0d216a1c6eb98`  
		Last Modified: Thu, 21 Oct 2021 21:56:12 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c031793c0b260a1cd280105d6113ddccf3f6b05b43ffcb9bc6d358322c2aaf88`  
		Last Modified: Tue, 02 Nov 2021 22:41:37 GMT  
		Size: 563.7 KB (563745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cced4bc76f6b8dce77bb51748a458d19c38ae5eccafbe9756265b68da36c837`  
		Last Modified: Fri, 05 Nov 2021 03:40:48 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84009f04738bd19cd3d458740e6c2c41c6426628a7987736c8ff4b6e9682851`  
		Last Modified: Fri, 05 Nov 2021 03:41:14 GMT  
		Size: 19.2 MB (19188641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:7330ce008d669ed57bbd8a9b4e131366c215032fb8dd2d6dd96766dd7831f433
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51335385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a60c141a54e8e89416fad6c21218eaeb4aabf4cf00ec47b18e87573b6dee71`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 20:48:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Oct 2021 20:48:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 14 Oct 2021 20:48:33 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Oct 2021 20:48:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Oct 2021 20:48:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 Oct 2021 20:48:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:48:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:48:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:31:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 16:16:04 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 16:16:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 16:16:06 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 16:16:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 16:16:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:23:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 16:23:23 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:23:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 16:23:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 16:23:25 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 16:23:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 16:23:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 16:23:28 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 16:23:29 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 17:13:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 17:13:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Nov 2021 21:36:10 GMT
COPY file:80d4bf27c2e7b39ab20a213acb94fe5d80ca22e3a11094d46fda4ad832320763 in /usr/local/bin/ 
# Fri, 05 Nov 2021 00:41:45 GMT
ENV DRUPAL_VERSION=9.2.8
# Fri, 05 Nov 2021 00:41:46 GMT
WORKDIR /opt/drupal
# Fri, 05 Nov 2021 00:42:03 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 05 Nov 2021 00:42:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988824645533e9f2462c2a2fc65988b7c65619d943ea77370ef098ddc6b019fa`  
		Last Modified: Thu, 14 Oct 2021 23:11:14 GMT  
		Size: 1.7 MB (1711538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e5bfd4fc6c9decc9649e8826be72c176d61dd7ff90c7c5363a2ffc32f5bb51`  
		Last Modified: Thu, 14 Oct 2021 23:11:14 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d281d60dbe28810fa660aac366b9fe5c9ef9eac047c112c6e57eccc5cbb375b`  
		Last Modified: Thu, 14 Oct 2021 23:11:14 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1005a6916b87e812615dc35912ec3c63325db556e85169413284efc04fff9a16`  
		Last Modified: Thu, 21 Oct 2021 16:40:00 GMT  
		Size: 10.7 MB (10733282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaef46a839b9131ef470719e35a00942ccdb899138e2bac4687b2b9876b997d`  
		Last Modified: Thu, 21 Oct 2021 16:39:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ec69f74fdde402f13cbf98c0669df45c57d63a2321409cfac506cdb019642`  
		Last Modified: Thu, 21 Oct 2021 16:40:32 GMT  
		Size: 14.5 MB (14501609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2e445ef524d7e29155ee218d86ce413e7bdecc49dbec24c964a5ec4b7dcb4f`  
		Last Modified: Thu, 21 Oct 2021 16:40:30 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f3f197e1f554184ddc107fc15f0019a4a579d7c8018914d8af510470a80fe`  
		Last Modified: Thu, 21 Oct 2021 16:40:30 GMT  
		Size: 17.5 KB (17488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14e81d6690a89a29fb524d2acd43c1634b93b161c5ce2da7bfc63541f01122a`  
		Last Modified: Thu, 21 Oct 2021 16:40:30 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da19a647e63ea03851c733b64cdc516c5fd995eda8dbd97a9653772a2848f24f`  
		Last Modified: Thu, 21 Oct 2021 17:36:48 GMT  
		Size: 1.9 MB (1892406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4fc278b7f32001f479ddaa8fb9daaa9331573a82f80dc46e622950f5d1ed455`  
		Last Modified: Thu, 21 Oct 2021 17:36:47 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435aef47dd58b5c5f232d7c871d068b4ee5cba6179f3d8bcbb7cf3aadb390cd9`  
		Last Modified: Tue, 02 Nov 2021 21:52:51 GMT  
		Size: 563.8 KB (563750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1e5ae8dd748888e0a2a0bbd5bc17a6e0577dd5dbd0881df3797c53970dabe7`  
		Last Modified: Fri, 05 Nov 2021 00:55:44 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ddec35bc537ca6e3d975d6e0f6fbe99ee58ff1011fd6116b20aa578c6b2d07`  
		Last Modified: Fri, 05 Nov 2021 00:55:49 GMT  
		Size: 19.2 MB (19189047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; 386

```console
$ docker pull drupal@sha256:bd3b0f313160658ff6c165bffaff2085ac3708635aff4658bbbb741e41e77261
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53109940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b048ddd4c9b7b2bb8ab72a1734d8c079b8450d59f24a2455af7577760613b22`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:43:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 31 Aug 2021 23:43:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 31 Aug 2021 23:43:21 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 31 Aug 2021 23:43:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 31 Aug 2021 23:43:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 31 Aug 2021 23:43:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 31 Aug 2021 23:43:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 31 Aug 2021 23:43:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 00:02:00 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 17:04:25 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 17:04:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 17:04:25 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 17:04:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 17:04:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 17:18:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 17:18:14 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 17:18:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 17:18:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 17:18:16 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 17:18:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 17:18:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 17:18:17 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 17:18:17 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 18:11:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 18:11:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Oct 2021 18:11:40 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Mon, 08 Nov 2021 20:38:50 GMT
ENV DRUPAL_VERSION=9.2.8
# Mon, 08 Nov 2021 20:38:51 GMT
WORKDIR /opt/drupal
# Mon, 08 Nov 2021 20:39:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 08 Nov 2021 20:39:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6dcde6dbfafb635836f32343bf73785cac3226c7dafda10ccc055161d4a7a3`  
		Last Modified: Wed, 01 Sep 2021 01:30:59 GMT  
		Size: 1.8 MB (1804920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0969b4b384f8446c0d8ecaaba87fab3da9e79620f0d1a2ea48003c985346ea76`  
		Last Modified: Wed, 01 Sep 2021 01:30:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318cb5a6ed97f1ae3a136dd27e290c71e8c5d668028cbfea14aaf90ad4cfec32`  
		Last Modified: Wed, 01 Sep 2021 01:30:58 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbcc3cb8d6d9f028fda7c383326b29747f3affdc51ec39cd3dcd838fc4c9505`  
		Last Modified: Thu, 21 Oct 2021 17:39:47 GMT  
		Size: 10.7 MB (10733533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ed3155a25826d07596e9ef40815426a9613db72688141e7456dbe70ec1b986`  
		Last Modified: Thu, 21 Oct 2021 17:39:45 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1432efbd5bd79741b471b955b21996e4dd1968c19d2dd7f24412de51bb715b`  
		Last Modified: Thu, 21 Oct 2021 17:40:27 GMT  
		Size: 15.7 MB (15663850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d295bb089c7f2df7de6f6d220e81742257b01c2ddce516274b0b8b873df6845d`  
		Last Modified: Thu, 21 Oct 2021 17:40:23 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8dbfab5700380034e0f358f1f4b9995e797a410a2f8e7009b9d172475112da`  
		Last Modified: Thu, 21 Oct 2021 17:40:23 GMT  
		Size: 17.6 KB (17621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1b011d45419ccae43894e9e0ad16c89537871dff9baf1543a52a8b3cd756b6`  
		Last Modified: Thu, 21 Oct 2021 17:40:23 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc165a9262012440bae3e2f20d4a54a1ec7a6372c3612fef091d572e7bd69990`  
		Last Modified: Thu, 21 Oct 2021 18:27:53 GMT  
		Size: 2.3 MB (2313805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73931f95af3fbf9f17e87dcef859510b38623ca6ef1647c0904fe34fdf0d2a3d`  
		Last Modified: Thu, 21 Oct 2021 18:27:52 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a72c6d1ffaa6e7281058b84a75297e779e8ac492816e80b1c0e30d3e09f92f`  
		Last Modified: Thu, 21 Oct 2021 18:27:53 GMT  
		Size: 553.2 KB (553183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac23f8d06b02a1f6c444a8058c3e66421eeb65b52618ba9d549e540fe39073`  
		Last Modified: Mon, 08 Nov 2021 20:55:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedfdfa85c699204c8bb54ec597a2d3d5ac832e2781c77989705a0e8911b45b`  
		Last Modified: Mon, 08 Nov 2021 20:55:40 GMT  
		Size: 19.2 MB (19188561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; ppc64le

```console
$ docker pull drupal@sha256:946a54140ba8ed16ddd0919dc6655237dfcf5984798f991b10f030f9c1854b1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53211584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c23a00ff717a4d3abd4e645ae184ceb67057119e93e89d30bc133e4092d811cb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:37:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 11:37:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 11:37:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 11:37:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 11:37:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 11:37:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 11:38:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 11:38:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 11:51:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 16:16:38 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 16:16:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 16:16:42 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 16:17:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 16:17:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:27:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 16:27:09 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:27:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 16:27:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 16:27:17 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 16:27:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 16:27:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 16:27:26 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 16:27:29 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 20:39:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 20:39:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Nov 2021 23:55:58 GMT
COPY file:80d4bf27c2e7b39ab20a213acb94fe5d80ca22e3a11094d46fda4ad832320763 in /usr/local/bin/ 
# Fri, 05 Nov 2021 02:49:51 GMT
ENV DRUPAL_VERSION=9.2.8
# Fri, 05 Nov 2021 02:49:56 GMT
WORKDIR /opt/drupal
# Fri, 05 Nov 2021 02:50:24 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 05 Nov 2021 02:50:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280fcf6c136467410ce39cbedb1567e6594635bcfb69b3408ebe41740112baf9`  
		Last Modified: Wed, 01 Sep 2021 12:50:23 GMT  
		Size: 1.8 MB (1753345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ffbefc6a72f5a7251be574aaf2b8ab0a340146a826cd12dd61bfef1a34f3ea`  
		Last Modified: Wed, 01 Sep 2021 12:50:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698662ec601124d3e71f3d6b5953ef4d8e2a14f3ead80a153d1133e3f65ee8d7`  
		Last Modified: Wed, 01 Sep 2021 12:50:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097334dcb0133b68a16c1f92016ead30fb20898394d9c333bbb332687c6a3d6f`  
		Last Modified: Thu, 21 Oct 2021 16:45:28 GMT  
		Size: 10.7 MB (10733526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17db28143d6b823b117850fe89d837794d8300a81829e7fb08a633d8db6a39e`  
		Last Modified: Thu, 21 Oct 2021 16:45:27 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890a97385ec2b74d136307cf352ec4b177e57b493d99bdcc1f74645f228bd9a7`  
		Last Modified: Thu, 21 Oct 2021 16:46:09 GMT  
		Size: 16.1 MB (16058179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6768d730a0045ac08d2c03ca2dcd4e2b554e02ff765869803072abf4f2ffaf1e`  
		Last Modified: Thu, 21 Oct 2021 16:46:05 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a697380fce69b714bd57cee366301b9b9b9dddf9070981c9fc12b14c9d7b05b`  
		Last Modified: Thu, 21 Oct 2021 16:46:05 GMT  
		Size: 17.6 KB (17623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34390115e3df79b77fb5da4385aadb56d1e27b9f37cc1a58b324cbc5d78dfe2a`  
		Last Modified: Thu, 21 Oct 2021 16:46:05 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b558459a5c46c3b7df4a6c6c6b78b29c55f9a1b323361b576027d595be571dc5`  
		Last Modified: Thu, 21 Oct 2021 21:22:21 GMT  
		Size: 2.1 MB (2068345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290bc01835527bd74396cc16cd5bec2f4fff9ad1583872e3e71b0f6a6a4ca5a`  
		Last Modified: Thu, 21 Oct 2021 21:22:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37e652de81d2b882d06201b9e18b5716c882e6c33ba8f338bebd26eabd0c7b1`  
		Last Modified: Wed, 03 Nov 2021 00:21:34 GMT  
		Size: 563.8 KB (563750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51674e8a8d2ee415c8d97e88eb3a3057895171d430ac80b79cb9ca78b723d29e`  
		Last Modified: Fri, 05 Nov 2021 03:09:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef41e6afd703864a9d1eb68617a332cbc9ac6f4bb84e2facb95023ae2333849`  
		Last Modified: Fri, 05 Nov 2021 03:10:29 GMT  
		Size: 19.2 MB (19188624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.0-fpm-alpine3.13` - linux; s390x

```console
$ docker pull drupal@sha256:c6dc2adf8cdb20c39fe0083d98342c1ddfc3d882e8a065b1ddbaaae54e997926
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51170234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f335101bdf8f19950458ccd9c9125eef94f846731f89ddfb347d0842dca8348`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Sep 2021 01:15:21 GMT
ADD file:def74c9e73d87d3c8b94cc0200f2723aea3a7462f8d2e0852db9da25c19855ac in / 
# Wed, 01 Sep 2021 01:15:22 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 13:38:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 13:38:53 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 13:38:54 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 13:38:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 13:38:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 13:38:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 13:38:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 13:38:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 13:51:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 21 Oct 2021 16:15:16 GMT
ENV PHP_VERSION=8.0.12
# Thu, 21 Oct 2021 16:15:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.12.tar.xz.asc
# Thu, 21 Oct 2021 16:15:17 GMT
ENV PHP_SHA256=a501017b3b0fd3023223ea25d98e87369b782f8a82310c4033d7ea6a989fea0a
# Thu, 21 Oct 2021 16:15:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 21 Oct 2021 16:15:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:22:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Oct 2021 16:22:04 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 21 Oct 2021 16:22:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Oct 2021 16:22:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Oct 2021 16:22:05 GMT
WORKDIR /var/www/html
# Thu, 21 Oct 2021 16:22:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Oct 2021 16:22:06 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Oct 2021 16:22:06 GMT
EXPOSE 9000
# Thu, 21 Oct 2021 16:22:06 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 17:06:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Oct 2021 17:06:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 02 Nov 2021 22:13:22 GMT
COPY file:80d4bf27c2e7b39ab20a213acb94fe5d80ca22e3a11094d46fda4ad832320763 in /usr/local/bin/ 
# Fri, 05 Nov 2021 00:43:45 GMT
ENV DRUPAL_VERSION=9.2.8
# Fri, 05 Nov 2021 00:43:45 GMT
WORKDIR /opt/drupal
# Fri, 05 Nov 2021 00:43:56 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 05 Nov 2021 00:44:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c1d78e8a87395f597d24b8eb78423ccdcfd404846906154e15aea8be9541c3ae`  
		Last Modified: Wed, 01 Sep 2021 01:16:19 GMT  
		Size: 2.6 MB (2604390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b7100aca97f69d9b374cc43f6b6e4c82448af53f0e220cb97a17a19eb17faa`  
		Last Modified: Wed, 01 Sep 2021 14:50:46 GMT  
		Size: 1.8 MB (1767631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac98bfca5f51191af2eca8072c19cab759e1d00591e268da0b641f6fd19e0d87`  
		Last Modified: Wed, 01 Sep 2021 14:50:45 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b73a29d7b83cfc931d5858b0f1c851817e4e5238d98d1240baae505cf5c70f`  
		Last Modified: Wed, 01 Sep 2021 14:50:45 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156980d7100829032b3dc120046551fec14bdd42e9dc4843eef35ae59ea3cfdf`  
		Last Modified: Thu, 21 Oct 2021 16:38:17 GMT  
		Size: 10.7 MB (10733538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4355f420367fb8fedab0b83abd7de3d5a70e09e75025efacd42486fe07a2bf06`  
		Last Modified: Thu, 21 Oct 2021 16:38:16 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6838c07893c469d5fad2bf88ca8775fa43aeae24f0e00f396d2db53fe8712080`  
		Last Modified: Thu, 21 Oct 2021 16:38:39 GMT  
		Size: 14.3 MB (14347516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb3c3a83260df44420a657c0da181ba30bf99ad3c1e2a399536d32d6d4d42a0`  
		Last Modified: Thu, 21 Oct 2021 16:38:37 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75975a85aaee0268426fd97ec5aaabc7f31e17e2860de614b892c3f8e43042f8`  
		Last Modified: Thu, 21 Oct 2021 16:38:37 GMT  
		Size: 17.6 KB (17633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecae2b43938c1d67ac4fd8645d5d3163d7f398ff842c104bc5f903f2e9b7346`  
		Last Modified: Thu, 21 Oct 2021 16:38:37 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18f5a7f5d321279dcb71fb1451b2704ca501e38cc736f64894f83a2ce1ba4e6`  
		Last Modified: Thu, 21 Oct 2021 17:19:06 GMT  
		Size: 1.9 MB (1933823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0982ec9eac6330b176e18b635ec997e87f94ce73e57392e304b6601938bbd19`  
		Last Modified: Thu, 21 Oct 2021 17:19:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e374c55df6891667568777138638b51c0023a07559a3bb80f053afd1b25a2a2`  
		Last Modified: Tue, 02 Nov 2021 22:32:33 GMT  
		Size: 563.7 KB (563749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cc25ffc5ac55ad4b507422b3e6b9563591f289a63af87fcb2ab519ed7fc102`  
		Last Modified: Fri, 05 Nov 2021 00:56:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3fc7946b7d17aa2a0b0a8d1e39efc43dbde03c5065f1bf5180916cab9fe094`  
		Last Modified: Fri, 05 Nov 2021 00:56:52 GMT  
		Size: 19.2 MB (19188585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
