## `drupal:10-fpm-alpine3.18`

```console
$ docker pull drupal@sha256:eb800b98dbc44b92d366d9cef08477cd958eab96d142b8dfa121f59b059e0b2c
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

### `drupal:10-fpm-alpine3.18` - linux; amd64

```console
$ docker pull drupal@sha256:72a35099d8c3cb0f9ee4c255ad13b594827f0a9f6fc0a8afb38d80e5b0aac567
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51631893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6367e0c169f9cf327a67ff55491e0e490705e07ba181190e0519f4e5f06cd72`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:31:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:31:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:31:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:31:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:31:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:31:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:31:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:31:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 00:54:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 00:54:34 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 00:54:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 00:54:34 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 00:54:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 00:54:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:01:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 01:01:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:01:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 01:01:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 01:01:58 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 01:01:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 01:01:59 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 01:01:59 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 01:01:59 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 07:27:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:27:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 07:27:40 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:27:40 GMT
ENV DRUPAL_VERSION=10.0.9
# Thu, 15 Jun 2023 07:27:40 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 07:27:50 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 07:27:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f034080c2b5d3afb2ec354e2b425f48df6326f28bcf3d2cee4ed50b9721ba482`  
		Last Modified: Thu, 15 Jun 2023 02:07:05 GMT  
		Size: 2.7 MB (2659635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8701d6f7d5844dd4fa64c17ce3e1999f152f0dbfa3ea704bf38e8617e6b4d5`  
		Last Modified: Thu, 15 Jun 2023 02:07:05 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259e9197ff8b826653ac60962d424d223ae725c1368f3fbd6efe6853200e945c`  
		Last Modified: Thu, 15 Jun 2023 02:07:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16e442da9b3fb4490b11e4664c414090d1113b974cc31af75dbfb1d5d8c4046`  
		Last Modified: Thu, 15 Jun 2023 02:08:53 GMT  
		Size: 12.0 MB (12037914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82868e6e9750585aa5ba0a2a2583fcf1d82fc3bd489f13340731940955d56483`  
		Last Modified: Thu, 15 Jun 2023 02:08:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1f0c77ff7f88374c8b8d10c73f3b112f9156ce9d6cd73c4e9562fdb747146b`  
		Last Modified: Thu, 15 Jun 2023 02:09:35 GMT  
		Size: 12.7 MB (12693419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21a98cab6dcc360269527e2e4332f204d0d006dfaae8e0f19a649b1a69bf242`  
		Last Modified: Thu, 15 Jun 2023 02:09:33 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756e46c6b2a96d3f31a23077ef6a7a40f6f1d14659fd3be219f0f5540915a7a4`  
		Last Modified: Thu, 15 Jun 2023 02:09:33 GMT  
		Size: 18.9 KB (18937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e1316337e692b14e56fc94be1a648d6c27d37140f6f0a85f8b1b32d9f6564b`  
		Last Modified: Thu, 15 Jun 2023 02:09:33 GMT  
		Size: 9.2 KB (9176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1b4eaed79acd2dcfab8aca6ded609fc874e3bbff6e253f2b64af9adaea9231`  
		Last Modified: Thu, 15 Jun 2023 07:38:04 GMT  
		Size: 2.4 MB (2436496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2869081869f5c0bda1f3c4a7b117e5f058754ee8b15eb493dd94db89d55843b1`  
		Last Modified: Thu, 15 Jun 2023 07:38:04 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb07085a47a5fbe0e351717a31156ee3282f94bb2eebc161e364d9edd8bcb75`  
		Last Modified: Thu, 15 Jun 2023 07:38:04 GMT  
		Size: 698.2 KB (698236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7969311c8d2e45595f1b9d5b582b986569df97f7c15c278d2789c6990d815bf8`  
		Last Modified: Thu, 15 Jun 2023 07:38:04 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1991d787d34d3c55d7e68d7a8558efebd640fcaee4e59a6c899790ddb11fdc5`  
		Last Modified: Thu, 15 Jun 2023 07:38:08 GMT  
		Size: 17.7 MB (17675267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; arm variant v6

```console
$ docker pull drupal@sha256:2e11056e7944c7ac16ca81f56d733250fa33dd32056ac48b48090a9327322a97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49712376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb1201e0cce37f2308db1d85fbcac3020efce1dd9cd844e11833c36f8a977b7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:03:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:03:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:03:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:03:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:03:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:03:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:03:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:03:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 00:21:56 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 00:21:56 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 00:21:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 00:21:56 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 00:22:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 00:22:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:27:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 00:27:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:27:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 00:27:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 00:27:23 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 00:27:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 00:27:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:27:23 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 00:27:24 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 07:36:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:36:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 07:36:11 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:36:11 GMT
ENV DRUPAL_VERSION=10.0.9
# Thu, 15 Jun 2023 07:36:11 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 07:36:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 07:36:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c974e2f4fb5afd0ccf2987ea9cdb17437ec18fae29ffb9fc867ac3086eb74400`  
		Last Modified: Thu, 15 Jun 2023 01:17:09 GMT  
		Size: 2.7 MB (2664702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64a2d84af76d29961595fccdcdf8d0e78b788f70e833458794d041be66462b5`  
		Last Modified: Thu, 15 Jun 2023 01:17:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e225c1eaef0162b3af2e6f6a0e68d0597a6d17226f086e1a5ee69dcd2e5248d`  
		Last Modified: Thu, 15 Jun 2023 01:17:09 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4171f2e23ab10d03571b8d3815993ca6fe2b989ec1751398d3c1a0b630dd65`  
		Last Modified: Thu, 15 Jun 2023 01:18:44 GMT  
		Size: 12.0 MB (12037906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fc47b2db36095f6a5d9850980abdfd93b9598ea2b3cbeed640f3006299a2e`  
		Last Modified: Thu, 15 Jun 2023 01:18:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a768ced5302b2ad43b38fc91d2a360ed7404bdd841151b72f709ef4f9e43a7`  
		Last Modified: Thu, 15 Jun 2023 01:19:26 GMT  
		Size: 11.6 MB (11605532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2590d34d7d8d14b1751f0904cdc31678caf761b0f8978152da1da59d19f3468f`  
		Last Modified: Thu, 15 Jun 2023 01:19:24 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146d1d7348cdf1e3f4166fda6973aa3bff7eed37bf7ddffde003e05cdcb77e41`  
		Last Modified: Thu, 15 Jun 2023 01:19:23 GMT  
		Size: 18.7 KB (18744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa5e8ef20a1378f1e25e5aaa56598e2e995bdfac9089d27556c3af94fb110e9`  
		Last Modified: Thu, 15 Jun 2023 01:19:23 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f35bf403dab24f16072d5078c3586663beab3c4a0603504aaebc33f79958c3`  
		Last Modified: Thu, 15 Jun 2023 07:42:00 GMT  
		Size: 1.9 MB (1854550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590aa09b9e9e067c17e216ecc2800be0d5938b09a15a6e5c90fc39eb7e39a092`  
		Last Modified: Thu, 15 Jun 2023 07:42:00 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96958b49f44229c081ec279752671aa08572b2a3e115d57ac1c84b7f280034`  
		Last Modified: Thu, 15 Jun 2023 07:42:00 GMT  
		Size: 698.2 KB (698237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697a78f548c36a60dfd4f42f06142165ef17238f683d19c764c10afd1dad673d`  
		Last Modified: Thu, 15 Jun 2023 07:41:59 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137dc66747566a40d32d0410f5330c532b8250f71162a45dc6032b3ef5bcf1a8`  
		Last Modified: Thu, 15 Jun 2023 07:42:05 GMT  
		Size: 17.7 MB (17675247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; arm variant v7

```console
$ docker pull drupal@sha256:b81f41a163decaf023341bfebda9b348e2f45daffbf5ba26285eeb8a9fb8901b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48411751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bcfd487610c7315a7864c643f2012fcd29737a95a251d66f088e0dc29ff525d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:41:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 05:41:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 05:41:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 05:41:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 05:41:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 05:41:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 05:41:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 05:41:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 05:57:26 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 05:57:26 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 05:57:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 05:57:26 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 05:57:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 05:57:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:02:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 06:02:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:02:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 06:02:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 06:02:26 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 06:02:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 06:02:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:02:26 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 06:02:26 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 10:03:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 10:03:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 10:03:02 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 10:03:02 GMT
ENV DRUPAL_VERSION=10.0.9
# Thu, 15 Jun 2023 10:03:02 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 10:03:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 10:03:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fcad4bb8996a5b45e9295adfb95c371938b842eb57e046b2913e94204a7f33`  
		Last Modified: Thu, 15 Jun 2023 06:52:24 GMT  
		Size: 2.5 MB (2502362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2cccda84c43168533736f637359fef9f6288fd02a44c5e793caaaa24105477`  
		Last Modified: Thu, 15 Jun 2023 06:52:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19901d84d4d52625e92590e32d9e2621e75c0beb01f75489bce2608d20f1c7ba`  
		Last Modified: Thu, 15 Jun 2023 06:52:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4ee4411084b57f61076fbd40a42217fbbbc54afd490573c4a6d7850a44a74e`  
		Last Modified: Thu, 15 Jun 2023 06:54:05 GMT  
		Size: 12.0 MB (12037921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d5f9155c1ca45d7c577c010490c88cbf92ff3bcc295e37a0e9db8b8b61fb1`  
		Last Modified: Thu, 15 Jun 2023 06:54:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a0028c65135e73adc24464b626d6961e2c83017ccbe7f3d4e8166807c8805e`  
		Last Modified: Thu, 15 Jun 2023 06:54:45 GMT  
		Size: 10.8 MB (10845942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894721e2305afcef2a81121af96a9c63df5892eb1c2fcf58f68a2b22a7a18f7c`  
		Last Modified: Thu, 15 Jun 2023 06:54:43 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8357b9bde1222a1fe0d1834dc3d4c65b45220715c47401ac606f1272c21a99`  
		Last Modified: Thu, 15 Jun 2023 06:54:43 GMT  
		Size: 18.8 KB (18762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4ea6ce5db74f8fec3d3053dec7fe664d71b5711dba6251e738f6beed903616`  
		Last Modified: Thu, 15 Jun 2023 06:54:43 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828f64a27de968e0e12fe489d2196819dbdc180310646918d59c85367720b297`  
		Last Modified: Thu, 15 Jun 2023 10:11:19 GMT  
		Size: 1.7 MB (1720592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e690df86d93c8893406fecdbccf9934e94543d254972e2bee7972c4fc67eaf3`  
		Last Modified: Thu, 15 Jun 2023 10:11:19 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5196b67537afa7304dc797dff80d0337729f1820890fa72117dbde0ecdfcd6dc`  
		Last Modified: Thu, 15 Jun 2023 10:11:19 GMT  
		Size: 698.2 KB (698239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc023847d3d4cf839bc48f0a9fbd0e49c4e7d19e628056bee3062c55c2725a7`  
		Last Modified: Thu, 15 Jun 2023 10:11:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c957a5c22ecc13ec5f7b63e901a04f63570c6a85506d565495fe0f96a7b7155`  
		Last Modified: Thu, 15 Jun 2023 10:11:24 GMT  
		Size: 17.7 MB (17675316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:f4ffddc00ffabd4a7b0acef5c0e161b1209c138e52f4919ec671056fc8750501
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51943863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda93b1d132b1d81edda2ec055614fd6239f2230d74906c033357314836bdf59`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:05:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 03:05:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 03:05:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 03:05:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 03:05:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 03:05:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:05:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:05:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 03:30:20 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 03:30:20 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 03:30:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 03:30:20 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 03:30:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 03:30:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:37:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 03:37:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 03:37:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 03:37:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 03:37:48 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 03:37:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 03:37:48 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 03:37:48 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 03:37:48 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 08:07:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 08:07:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 08:07:33 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 08:07:33 GMT
ENV DRUPAL_VERSION=10.0.9
# Thu, 15 Jun 2023 08:07:33 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 08:07:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 08:07:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cbf4f33af4ff20fa90638cea5f48dda44f171afe80c0ca68a40b5c67ee1102`  
		Last Modified: Thu, 15 Jun 2023 04:39:12 GMT  
		Size: 2.7 MB (2696456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0262450c79d37bc5398bf1154c4bb2681100ef9caf7e008c5d0bd06c3d840a7`  
		Last Modified: Thu, 15 Jun 2023 04:39:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca0f0b2514d4e2b8323c60eece66557c89959c380362deb6862fe5ffe3ad14`  
		Last Modified: Thu, 15 Jun 2023 04:39:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a31969c464d209f6338c19ffcc3ffa5cd1b719cc1d51d8d17bb436368424f`  
		Last Modified: Thu, 15 Jun 2023 04:40:50 GMT  
		Size: 12.0 MB (12037901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22ecd80207b141e59fa3a40ad129bbced191c30b0cf8f2be2d324301f30587f`  
		Last Modified: Thu, 15 Jun 2023 04:40:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e4497f71db74dd78d5ae574d84bccdc90f47b8a876098885243eb70ac8b2f`  
		Last Modified: Thu, 15 Jun 2023 04:41:29 GMT  
		Size: 12.8 MB (12770377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1151d5ab28fcb76884fe12db8006d68e2682a6dfa99030911f77b6fa31021ae1`  
		Last Modified: Thu, 15 Jun 2023 04:41:27 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571fb0d265dfe7969fbbe3e1dea15866dd50c6bda97511518badca9e1a8c6ef0`  
		Last Modified: Thu, 15 Jun 2023 04:41:27 GMT  
		Size: 18.7 KB (18702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69f93ae2f10ad6e6868c046ea56fec3dc600318ffc1b1bd07d969213b3bbfe1`  
		Last Modified: Thu, 15 Jun 2023 04:41:28 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbb89877b562eaf1828cfdeca214d32008e6823692672c177af948963023a24`  
		Last Modified: Thu, 15 Jun 2023 08:17:27 GMT  
		Size: 2.7 MB (2703545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e00b023cb139a3da16b0dc656a124477efdfa6e33eea2db247994783daf9a8`  
		Last Modified: Thu, 15 Jun 2023 08:17:27 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada270b4cd753f9094b11e5bbb759dd95e5a4b2c8e54d611bdee9267ae435ff4`  
		Last Modified: Thu, 15 Jun 2023 08:17:27 GMT  
		Size: 698.2 KB (698237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e285e7457323f98735f67ad58e1f51fc40a97dfb885d49168bc0554337eafaed`  
		Last Modified: Thu, 15 Jun 2023 08:17:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7751fb9164f2b2e3bd1f22b2a582e7aaae4af1f258a92d0b2f892b99f6ba9149`  
		Last Modified: Thu, 15 Jun 2023 08:17:30 GMT  
		Size: 17.7 MB (17675285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; 386

```console
$ docker pull drupal@sha256:cac5db658c84786867f62b4e570a8fabc3f4e0fe6d480544b71c9941ac6c441a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51697262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62b74e5004759907f0991dab9e849479652c07a30f38cc0344bb44677d1c412`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:26:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 06:26:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 06:26:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 06:26:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 06:26:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 06:26:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 06:26:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 06:26:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 07:05:14 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 15 Jun 2023 07:05:14 GMT
ENV PHP_VERSION=8.2.7
# Thu, 15 Jun 2023 07:05:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Thu, 15 Jun 2023 07:05:14 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Thu, 15 Jun 2023 07:06:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 07:06:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:18:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 07:18:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:18:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 07:18:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 07:18:25 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 07:18:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 07:18:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 07:18:25 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 07:18:25 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 10:33:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 10:33:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 10:33:14 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 10:33:14 GMT
ENV DRUPAL_VERSION=10.0.9
# Thu, 15 Jun 2023 10:33:14 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 10:33:26 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 10:33:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686addfe363578d7327e190b5b07780e2e046ab88a2d36c1d45bf9433e6dcd5a`  
		Last Modified: Thu, 15 Jun 2023 09:10:03 GMT  
		Size: 2.7 MB (2699507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcfa11cca4a6fe8bb794ac07926f350ef4be9309437a2e4665ef8a89b425b54`  
		Last Modified: Thu, 15 Jun 2023 09:10:03 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1a40c4c1022edb58f063eb71a5482c5b66ab16c804b7b215db18d809affb5b`  
		Last Modified: Thu, 15 Jun 2023 09:10:03 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766d6bb223f71c05b90f5610c2ebe69286860b8ed040e7cd0f199cb6110c0746`  
		Last Modified: Thu, 15 Jun 2023 09:12:05 GMT  
		Size: 12.0 MB (12037912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557892a7f3ab803b6a569af85965f4e8e6f392dee16c55a0fb319446504d3566`  
		Last Modified: Thu, 15 Jun 2023 09:12:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf0fd8d030ccd83ac2c5332e05ef79cca7b9c7c409914bf790c5c2ff2fa6445`  
		Last Modified: Thu, 15 Jun 2023 09:12:49 GMT  
		Size: 12.9 MB (12891183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e70d72cb98e7e1990f7b3b6888bb42f0db3c6ca9e1d2eb08de8bd6280eeba`  
		Last Modified: Thu, 15 Jun 2023 09:12:46 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05650c6f1a9e92a53e80ce517daeb7a602cc5c14be02f4168aa362bb05e7fa3`  
		Last Modified: Thu, 15 Jun 2023 09:12:46 GMT  
		Size: 18.9 KB (18927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a4fdca3f4dc74d1609d5a6302584eeaf49b88e75bbf23625f440c73a9ea745`  
		Last Modified: Thu, 15 Jun 2023 09:12:46 GMT  
		Size: 9.2 KB (9180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cb178153b3e6f14933ffd0fb9836dd6d8bed068f8de5577e3c95dde14cfe6`  
		Last Modified: Thu, 15 Jun 2023 10:43:50 GMT  
		Size: 2.4 MB (2427999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0350dffd62d6dc9d9fb52992d3fc7c910248f60945d2d96ff1fcfb565077de1`  
		Last Modified: Thu, 15 Jun 2023 10:43:50 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f8758cfdc674a8a7a4e485b239937793628f4f543330cc54043984706913f8`  
		Last Modified: Thu, 15 Jun 2023 10:43:50 GMT  
		Size: 698.2 KB (698239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c7ce1072721a4c12e904407750345cbd077a39752e434b7f6edf81739b521b`  
		Last Modified: Thu, 15 Jun 2023 10:43:50 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cdd92140351661e3567b1ffeeac2fc7c461f7732b95176fd3a3c7478358271`  
		Last Modified: Thu, 15 Jun 2023 10:43:56 GMT  
		Size: 17.7 MB (17675429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; ppc64le

```console
$ docker pull drupal@sha256:42b04d2ce36e9ae788cd9f004cd0b2296fc734e1a8c086bef27fc27276f3cf0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.4 MB (54426382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7e75754e74335068dfa1cec606969be1bd9e1e897e5458eb4484fd5c1a6a588`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 21:29:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 May 2023 21:29:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 May 2023 21:29:12 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 May 2023 21:29:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 May 2023 21:29:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 11 May 2023 21:29:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 May 2023 21:29:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 May 2023 21:29:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 May 2023 21:29:15 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 09 Jun 2023 00:22:04 GMT
ENV PHP_VERSION=8.2.7
# Fri, 09 Jun 2023 00:22:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Fri, 09 Jun 2023 00:22:04 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Fri, 09 Jun 2023 00:22:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 00:22:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 09 Jun 2023 00:30:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 09 Jun 2023 00:30:07 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 09 Jun 2023 00:30:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 09 Jun 2023 00:30:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 09 Jun 2023 00:30:10 GMT
WORKDIR /var/www/html
# Fri, 09 Jun 2023 00:30:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 09 Jun 2023 00:30:11 GMT
STOPSIGNAL SIGQUIT
# Fri, 09 Jun 2023 00:30:11 GMT
EXPOSE 9000
# Fri, 09 Jun 2023 00:30:11 GMT
CMD ["php-fpm"]
# Fri, 09 Jun 2023 02:56:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 09 Jun 2023 02:56:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 12 Jun 2023 19:34:49 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Mon, 12 Jun 2023 19:34:49 GMT
ENV DRUPAL_VERSION=10.0.9
# Mon, 12 Jun 2023 19:34:50 GMT
WORKDIR /opt/drupal
# Mon, 12 Jun 2023 19:35:15 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 12 Jun 2023 19:35:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7ab64acf5d7892690b10023745d6938fb8b74120c8c60235a21cace67fff33`  
		Last Modified: Thu, 11 May 2023 22:28:19 GMT  
		Size: 2.7 MB (2728145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12ef25af3414555b87ae448bb8e85e3f3805ec3dc4ad68bde083f1e61ca3423`  
		Last Modified: Thu, 11 May 2023 22:28:18 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b6a996eabeeaa6829fb842ecc5a98a81553b1a9bba417dbcb837eca423720`  
		Last Modified: Thu, 11 May 2023 22:28:18 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a716d383c586649f1f13fdbd83d9dfa12e2fc35d62ebdf3046d4f7bc2d3d032e`  
		Last Modified: Fri, 09 Jun 2023 02:26:40 GMT  
		Size: 12.0 MB (12037883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d0083565e0eafbd70212f9319997828b55728d8717c4a763199b843dc99fcd`  
		Last Modified: Fri, 09 Jun 2023 02:26:39 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e5587aa9bdf670b7eca2bbb335d610703119b1a4c150f962d70d56df38fe9d`  
		Last Modified: Fri, 09 Jun 2023 02:27:31 GMT  
		Size: 15.6 MB (15611190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645f6b12b2bfb564fd1aeb7e6f9c6f25907142d9ea1c18b8b84c52875bdd5fe`  
		Last Modified: Fri, 09 Jun 2023 02:27:26 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bdb8da8c9a56da34d632d120b31a0dc75baecee398ed8f1517977bf7ceafcb`  
		Last Modified: Fri, 09 Jun 2023 02:27:26 GMT  
		Size: 18.8 KB (18765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962bfc9f73adcf64fdb0db286945510ebd25f18e9a10d179e549c344213f8487`  
		Last Modified: Fri, 09 Jun 2023 02:27:26 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3929c608be7ca032400e8d74140b677c6f463b7215aeafe1b2a31a764d82be1`  
		Last Modified: Fri, 09 Jun 2023 03:20:45 GMT  
		Size: 2.3 MB (2256931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506022d2ae9345d0add1787307f7363175bfa970f41cbadbb56397f4c06d10f7`  
		Last Modified: Fri, 09 Jun 2023 03:20:44 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec53d049906bd4e076f51986bdc322ce66c7e3d5aa0bd030e243a85d1a34d90e`  
		Last Modified: Mon, 12 Jun 2023 19:51:32 GMT  
		Size: 698.2 KB (698241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab367885904e757b3495f45260d5e4699947422923c98f73f69f7b578ba937c`  
		Last Modified: Mon, 12 Jun 2023 19:51:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23b0fa4719ff49feb30d135c5f3625685dd612b73aa6ca93b586ec2483e8bb`  
		Last Modified: Mon, 12 Jun 2023 19:51:52 GMT  
		Size: 17.7 MB (17675478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.18` - linux; s390x

```console
$ docker pull drupal@sha256:a526722b7603c8bfaf66397750730dcbf5296cf066006f75b3a4a13e91912872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52663568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158e25462195627fbd568adda1e02e2344892ae967774fa7d386cecded1e2238`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 20:10:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 May 2023 20:10:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 May 2023 20:10:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 May 2023 20:10:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 May 2023 20:10:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 11 May 2023 20:10:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 May 2023 20:10:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 May 2023 20:10:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 May 2023 20:10:58 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 09 Jun 2023 00:19:30 GMT
ENV PHP_VERSION=8.2.7
# Fri, 09 Jun 2023 00:19:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.7.tar.xz.asc
# Fri, 09 Jun 2023 00:19:30 GMT
ENV PHP_SHA256=4b9fb3dcd7184fe7582d7e44544ec7c5153852a2528de3b6754791258ffbdfa0
# Fri, 09 Jun 2023 00:19:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 00:19:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 09 Jun 2023 00:24:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 09 Jun 2023 00:24:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 09 Jun 2023 00:24:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 09 Jun 2023 00:24:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 09 Jun 2023 00:24:56 GMT
WORKDIR /var/www/html
# Fri, 09 Jun 2023 00:24:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 09 Jun 2023 00:24:57 GMT
STOPSIGNAL SIGQUIT
# Fri, 09 Jun 2023 00:24:57 GMT
EXPOSE 9000
# Fri, 09 Jun 2023 00:24:57 GMT
CMD ["php-fpm"]
# Fri, 09 Jun 2023 02:01:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 09 Jun 2023 02:01:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 12 Jun 2023 19:59:02 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Mon, 12 Jun 2023 19:59:02 GMT
ENV DRUPAL_VERSION=10.0.9
# Mon, 12 Jun 2023 19:59:02 GMT
WORKDIR /opt/drupal
# Mon, 12 Jun 2023 19:59:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 12 Jun 2023 19:59:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1229cbf44dd4d93ce3b40fc629fa6700457195d0080eb6e6d28096372f526093`  
		Last Modified: Thu, 11 May 2023 20:57:02 GMT  
		Size: 2.8 MB (2753025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997be929bbab1ac7c5ea596b8d8336fdc045fe9ced4c15b05bb8173b1f9b79a8`  
		Last Modified: Thu, 11 May 2023 20:57:02 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e9ef3515d879c1d5a2806852a344a3349ab8399604e5cdd2ca621b69cc8e4a`  
		Last Modified: Thu, 11 May 2023 20:57:02 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4984a7bbd3a0fe4e4b39bdaccf4d4528278f0485a8d4dd1a1af9b288e6d2141e`  
		Last Modified: Fri, 09 Jun 2023 01:36:54 GMT  
		Size: 12.0 MB (12037881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1f60a7e649590f2d968f2f4270e75da15dbd383a972dba4d50f090ae0307e2`  
		Last Modified: Fri, 09 Jun 2023 01:36:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4da2481041c30567d7cb9019a001a5cf0cb7e5164dfbfb436f8ac6574d37a1b`  
		Last Modified: Fri, 09 Jun 2023 01:37:17 GMT  
		Size: 14.2 MB (14241581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e184578cd85ed0667465e808e1ccfdbc3c7485c4151736892cb98eaabf1b7ec1`  
		Last Modified: Fri, 09 Jun 2023 01:37:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8aebc22ef461083d49fdb9b990d2a0512f67d227a3d5020a10645dfdc7161`  
		Last Modified: Fri, 09 Jun 2023 01:37:15 GMT  
		Size: 18.8 KB (18781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d661fbb2bf00872ff1379d42a6bc8568088e9dc6ba9c685d79c5a321fef1c1`  
		Last Modified: Fri, 09 Jun 2023 01:37:14 GMT  
		Size: 9.2 KB (9176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86346bb1f2043d3c8705cc4f3be31cf82f2fbad915b88ee465a462a8b809f73`  
		Last Modified: Fri, 09 Jun 2023 02:15:17 GMT  
		Size: 2.0 MB (1998357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97943575239bfa11d33eb458c01cee668316dcb37199edbaaeff2ea539decf1c`  
		Last Modified: Fri, 09 Jun 2023 02:15:16 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beaa74cba18b9bb160de771ead8bcc92d67938998b4a23023f47feae618215b2`  
		Last Modified: Mon, 12 Jun 2023 20:09:14 GMT  
		Size: 698.2 KB (698241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5802243932d92eb228551b8646c028db801af6170fc6e03e76720f5aa6a9f841`  
		Last Modified: Mon, 12 Jun 2023 20:09:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac3dde5516d0997c6a663a853aaa2ff62b042f48b83f250636242adfafb1c14`  
		Last Modified: Mon, 12 Jun 2023 20:09:18 GMT  
		Size: 17.7 MB (17675287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
