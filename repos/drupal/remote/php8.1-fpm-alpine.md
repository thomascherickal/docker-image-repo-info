## `drupal:php8.1-fpm-alpine`

```console
$ docker pull drupal@sha256:be5627db9cb8f0e57d77f77682d0efc62ac3fb0aa8a0ac3262be294c01db432c
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

### `drupal:php8.1-fpm-alpine` - linux; amd64

```console
$ docker pull drupal@sha256:48c3b0ffb1e62dc67d085c20b4b81b02eefe740fb88353d35152272406526ca8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55385672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8dbd0b573d05424ba546bb3ca6762f4a7762915912ce75717f3cc3735f3f909`
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
# Thu, 15 Jun 2023 01:17:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:39:19 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:39:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:39:19 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:39:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Aug 2023 22:39:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:46:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:46:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:46:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:46:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:46:21 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:46:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 04 Aug 2023 22:46:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Aug 2023 22:46:22 GMT
EXPOSE 9000
# Fri, 04 Aug 2023 22:46:22 GMT
CMD ["php-fpm"]
# Fri, 04 Aug 2023 23:49:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 04 Aug 2023 23:49:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Aug 2023 23:49:59 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:49:59 GMT
ENV DRUPAL_VERSION=10.1.2
# Fri, 04 Aug 2023 23:49:59 GMT
WORKDIR /opt/drupal
# Fri, 04 Aug 2023 23:50:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 04 Aug 2023 23:50:10 GMT
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
	-	`sha256:9c972ec96e340f54b126d0d6d9128e93e8cb46a8a2199f4991438e7d49ab64bf`  
		Last Modified: Fri, 04 Aug 2023 23:24:50 GMT  
		Size: 11.8 MB (11829764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc190f3b174006c9f6afa561c1b249eff3a9e42354c0ea15ed8eb92cd37cc4b`  
		Last Modified: Fri, 04 Aug 2023 23:24:48 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc82a5103878b271f52bd295364b454690bf759db60bd61d3409df147072e4fc`  
		Last Modified: Fri, 04 Aug 2023 23:25:16 GMT  
		Size: 15.8 MB (15824134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cb02067ba862fe2572c28c6ffc85ec249274dc585922af00e21399520b50e4`  
		Last Modified: Fri, 04 Aug 2023 23:25:14 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86209c23d26cc111d685b717fdf68f66cfdfa79c8b46ac3dcdbd1837d41150a`  
		Last Modified: Fri, 04 Aug 2023 23:25:14 GMT  
		Size: 19.0 KB (18973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cc19fdd526b94d393e7032fbe81e61d35f157df8bcd9941f11e7e82957093`  
		Last Modified: Fri, 04 Aug 2023 23:25:14 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563c0b789a3cf0426834362650bcafee76c756641241db9de965090adb7a1997`  
		Last Modified: Sat, 05 Aug 2023 00:01:29 GMT  
		Size: 2.4 MB (2435805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff462fdd1d235a45bb4e291fa3db916f1950b289ec45b84f9acc44adca2d0b45`  
		Last Modified: Sat, 05 Aug 2023 00:01:29 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cdc4abbaa8a54596cd32f57bb8c6064be6e8e5a8e199f966d9989b278c5fc6`  
		Last Modified: Sat, 05 Aug 2023 00:01:29 GMT  
		Size: 698.2 KB (698240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0b3438c6e8ff6ed7b0f50e787bcf9e4061829c03aeaddc461268543c1cfea`  
		Last Modified: Sat, 05 Aug 2023 00:01:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a705081be0264c09109891adc5caf909910fea074ad6318cec09e4aa790f92`  
		Last Modified: Sat, 05 Aug 2023 00:01:33 GMT  
		Size: 18.5 MB (18507424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull drupal@sha256:74e44c0621ecb39304924b238a0cf2869da5b9f7ee2700dd29feaf16b3287e37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53136432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1f2f2e8b1e10f4a17b129ce47bd8b6f194ce878715f937e8f83bd077f56a098`
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
# Thu, 15 Jun 2023 00:39:58 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:14:05 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:14:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:14:05 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:14:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Aug 2023 22:14:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:22:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:22:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:22:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:22:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:22:56 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:22:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 04 Aug 2023 22:22:57 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Aug 2023 22:22:58 GMT
EXPOSE 9000
# Fri, 04 Aug 2023 22:22:58 GMT
CMD ["php-fpm"]
# Fri, 04 Aug 2023 23:28:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 04 Aug 2023 23:28:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Aug 2023 23:28:44 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:28:44 GMT
ENV DRUPAL_VERSION=10.1.2
# Fri, 04 Aug 2023 23:28:44 GMT
WORKDIR /opt/drupal
# Fri, 04 Aug 2023 23:28:58 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 04 Aug 2023 23:28:58 GMT
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
	-	`sha256:948685876ad95da6c9c02572e74d7357a416b3f1d55601c4315b3b70e0cc975c`  
		Last Modified: Fri, 04 Aug 2023 22:59:49 GMT  
		Size: 11.8 MB (11829758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bde923dd130164520648ac3b429c51af16055258a69198810406cec87e7904`  
		Last Modified: Fri, 04 Aug 2023 22:59:48 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8493c5c226b64ecbf255b1423101b88c112eeed3295630feaf719ca0809d31f9`  
		Last Modified: Fri, 04 Aug 2023 23:00:26 GMT  
		Size: 14.4 MB (14416106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689f044ff30afb66f281e73ca43d2391b67d8e5e97d51dc3fa4f56281fd02f42`  
		Last Modified: Fri, 04 Aug 2023 23:00:23 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e024cc9e00d846b7a2608a93bb9bbde925edab53391ad911c112709f2aecc136`  
		Last Modified: Fri, 04 Aug 2023 23:00:23 GMT  
		Size: 18.8 KB (18792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0c1cd2967bd914825af4bd3a1a583dc1e9083dbc543bac1e4983569cefc14`  
		Last Modified: Fri, 04 Aug 2023 23:00:23 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf42da112fcfa2c1bb65e7a5d3dd4e5c8c062074f2afb1d5986b18329e35ce6`  
		Last Modified: Fri, 04 Aug 2023 23:32:45 GMT  
		Size: 1.8 MB (1844631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd4046c505324d7c1ef9c5c639f5d5641bdd2a580797768eb217da89b4be3f`  
		Last Modified: Fri, 04 Aug 2023 23:32:44 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33febe25f7d9f19cce5915ced256d013536f6dd53ec825bea6207ee27f1e6c25`  
		Last Modified: Fri, 04 Aug 2023 23:32:45 GMT  
		Size: 698.2 KB (698239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497a4a47b1e8bbe3e16935028df3f89524efbf24fc6e7587dd65c939e703fe11`  
		Last Modified: Fri, 04 Aug 2023 23:32:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e31d64a97b3132181ca0d5b3891e7360e1cd9cb5e6761a5325ace2ea9b85cf`  
		Last Modified: Fri, 04 Aug 2023 23:32:51 GMT  
		Size: 18.5 MB (18507029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull drupal@sha256:b989f0c54ba789b971e64db3b6a8406c0f4ec8fa09f3dbf0a31117f4dd55779c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51643751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfdbc6d35afbf79542c6f8ed8acdc0d56a36aaf8aba4840bf74696720df794e`
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
# Thu, 15 Jun 2023 06:13:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 23:31:50 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 23:31:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 23:31:50 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 23:31:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Aug 2023 23:31:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:37:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 23:37:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:37:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 23:37:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 23:37:22 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 23:37:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 04 Aug 2023 23:37:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Aug 2023 23:37:22 GMT
EXPOSE 9000
# Fri, 04 Aug 2023 23:37:22 GMT
CMD ["php-fpm"]
# Sat, 05 Aug 2023 00:31:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 05 Aug 2023 00:31:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:31:36 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Sat, 05 Aug 2023 00:31:36 GMT
ENV DRUPAL_VERSION=10.1.2
# Sat, 05 Aug 2023 00:31:36 GMT
WORKDIR /opt/drupal
# Sat, 05 Aug 2023 00:31:46 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 05 Aug 2023 00:31:47 GMT
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
	-	`sha256:29767d03bb61bf25cd49ed9aca9dfab979e48ccbec2937335742c58e3e7b25af`  
		Last Modified: Sat, 05 Aug 2023 00:09:28 GMT  
		Size: 11.8 MB (11829776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750c90529ea91679078b99ba28e9bf0da048d08e52d6f938cfc40ac800ddd15`  
		Last Modified: Sat, 05 Aug 2023 00:09:26 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0a834e72a1905752852c53cb1a370a5922f1c6c25ca2ed66ecc33c577945cd`  
		Last Modified: Sat, 05 Aug 2023 00:09:55 GMT  
		Size: 13.5 MB (13465395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c498c6d5393bd67db892b5c9be46d4238754ecb1a791331173d53681cd98c9`  
		Last Modified: Sat, 05 Aug 2023 00:09:53 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3d5244d7fcf9e19c6e4df8c22e1c812d7dd84d89a496eb36713ec43b187afd`  
		Last Modified: Sat, 05 Aug 2023 00:09:53 GMT  
		Size: 18.8 KB (18802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b081a0c0fc0070d435fd30eaaa9ca9eb4602acdf4b7446fbf082530062b7d1`  
		Last Modified: Sat, 05 Aug 2023 00:09:53 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740fa3931f2d03c6f255de7ed42d7ea59b1db852465a2cfdad68ffec4f9994f4`  
		Last Modified: Sat, 05 Aug 2023 00:41:27 GMT  
		Size: 1.7 MB (1709896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b453141907ae3e23143e7f75ae4dd2344ac971df0c8971e243565e0c690228fa`  
		Last Modified: Sat, 05 Aug 2023 00:41:25 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe2905ea551b1132a737cf68747f8a7fa6b9442c238874b02e964fc59ac467`  
		Last Modified: Sat, 05 Aug 2023 00:41:26 GMT  
		Size: 698.2 KB (698239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5fdfb1fe1a12874128645b9ec10099888843084028791569c9c999755e26e9`  
		Last Modified: Sat, 05 Aug 2023 00:41:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff3a301d079df03af91df73cdb95f8decb91f42d21c9977c83f45611355b7f0`  
		Last Modified: Sat, 05 Aug 2023 00:41:31 GMT  
		Size: 18.5 MB (18506956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:726406d2ee52c71a7a77f8eaeebbb68d36bba38d939ab5c408e73442e53c6cae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52330318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a349bc8582fd3e51e68eb8ebd4f4fe7f4aca895c791bbdefadf430e4b976a10`
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
# Thu, 15 Jun 2023 03:53:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Mon, 10 Jul 2023 23:50:42 GMT
ENV PHP_VERSION=8.1.21
# Mon, 10 Jul 2023 23:50:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.21.tar.xz.asc
# Mon, 10 Jul 2023 23:50:42 GMT
ENV PHP_SHA256=e634a00b0c6a8cd39e840e9fb30b5227b820b7a9ace95b7b001053c1411c4821
# Mon, 10 Jul 2023 23:50:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 10 Jul 2023 23:50:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:57:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 23:57:46 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:57:47 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 23:57:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 23:57:47 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 23:57:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 23:57:48 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 23:57:48 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 23:57:48 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 03:11:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 11 Jul 2023 03:11:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 03:11:32 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 03 Aug 2023 01:37:22 GMT
ENV DRUPAL_VERSION=10.1.2
# Thu, 03 Aug 2023 01:37:22 GMT
WORKDIR /opt/drupal
# Thu, 03 Aug 2023 01:37:30 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 03 Aug 2023 01:37:31 GMT
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
	-	`sha256:9c381c84274ecfc418f2bf0dab4406a97dc2ce4beeddcfe97444edc74c3145ec`  
		Last Modified: Tue, 11 Jul 2023 00:39:11 GMT  
		Size: 11.9 MB (11882762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b1b7e8ed928ad1aace7bccbabe161679119b6cba120241f72b5455b7744f9f`  
		Last Modified: Tue, 11 Jul 2023 00:39:10 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa90278d06f6d95544a9945ea4f5bf9599ef18561e9aadce2e9683dbbe38d2f`  
		Last Modified: Tue, 11 Jul 2023 00:39:35 GMT  
		Size: 12.5 MB (12481535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c827c056486ad76a3e9ba84dce50fa421f6a1bed50a4a92858833b6072f916e1`  
		Last Modified: Tue, 11 Jul 2023 00:39:33 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc837957f1c99beaf65470e7c28ff40041152f8c5221ef0a37c0cbe52aec2429`  
		Last Modified: Tue, 11 Jul 2023 00:39:34 GMT  
		Size: 18.7 KB (18707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63e612cdcee06cec3bb1b5e87706ec38663d380918c04ab0187f225d1a52624`  
		Last Modified: Tue, 11 Jul 2023 00:39:33 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c227affdd73e83ceaf1284cb562d39628ac8526b2558ed13c821be8bf55d4e08`  
		Last Modified: Tue, 11 Jul 2023 03:28:03 GMT  
		Size: 2.7 MB (2702615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f8a381be7fe7ea408f993cf74baa3309b07d8466bccd5e22d8f29258c073e0`  
		Last Modified: Tue, 11 Jul 2023 03:28:03 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9809b9b0741ea19224a096d033779f5cc694b706eb82bc40c5d09126473d77`  
		Last Modified: Tue, 11 Jul 2023 03:28:03 GMT  
		Size: 698.2 KB (698236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0d81bd454a02161aef933a17543fca5db5199f01d355359bab4a8972e01701`  
		Last Modified: Thu, 03 Aug 2023 01:47:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1354eceb50029530b0fbc55e5917f885e2233baf3bab34fa2834de482a2e51`  
		Last Modified: Thu, 03 Aug 2023 01:47:15 GMT  
		Size: 18.5 MB (18506950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; 386

```console
$ docker pull drupal@sha256:f44407b674fc86734afc19af58d19e025dccd9b96a2f4a471359814619564051
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52077288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c41b8e850488146a5f38bbf0532ee921b74aea4adedf39ab63c773655033875`
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
# Thu, 15 Jun 2023 07:44:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Mon, 10 Jul 2023 23:20:59 GMT
ENV PHP_VERSION=8.1.21
# Mon, 10 Jul 2023 23:20:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.21.tar.xz.asc
# Mon, 10 Jul 2023 23:20:59 GMT
ENV PHP_SHA256=e634a00b0c6a8cd39e840e9fb30b5227b820b7a9ace95b7b001053c1411c4821
# Mon, 10 Jul 2023 23:21:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 10 Jul 2023 23:21:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:32:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 10 Jul 2023 23:32:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 10 Jul 2023 23:32:59 GMT
RUN docker-php-ext-enable sodium
# Mon, 10 Jul 2023 23:32:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 10 Jul 2023 23:33:00 GMT
WORKDIR /var/www/html
# Mon, 10 Jul 2023 23:33:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 10 Jul 2023 23:33:00 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Jul 2023 23:33:00 GMT
EXPOSE 9000
# Mon, 10 Jul 2023 23:33:00 GMT
CMD ["php-fpm"]
# Tue, 11 Jul 2023 01:51:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 11 Jul 2023 01:51:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 11 Jul 2023 01:51:34 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 03 Aug 2023 00:41:28 GMT
ENV DRUPAL_VERSION=10.1.2
# Thu, 03 Aug 2023 00:41:29 GMT
WORKDIR /opt/drupal
# Thu, 03 Aug 2023 00:41:40 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 03 Aug 2023 00:41:41 GMT
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
	-	`sha256:18d1a8569eb1415d3c5cf0962c09a3bdf9f14b2528ed4a0516c66099461459c7`  
		Last Modified: Tue, 11 Jul 2023 00:36:35 GMT  
		Size: 11.9 MB (11882775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265d239218e5e06ca3bdbb2b6f0e82e111fda3a6d7cfa21bc2bc72f3f35cb65c`  
		Last Modified: Tue, 11 Jul 2023 00:36:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8e899a088bdb8ebf00ffa17c1d5bbde7671a01c1b188a466c837a4ccf27d47`  
		Last Modified: Tue, 11 Jul 2023 00:37:03 GMT  
		Size: 12.6 MB (12597801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f44f0bc44abfe59ceef273679fc1d89b6a0896036d03e8f130521f83846aca`  
		Last Modified: Tue, 11 Jul 2023 00:37:00 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f9e0e8de4edf1233497a4b359c50eb3c3a0a1b597582f869833610d3a8bb1e`  
		Last Modified: Tue, 11 Jul 2023 00:37:00 GMT  
		Size: 18.9 KB (18929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35ea54ec7b7bce7f908a2d25036567a882e378b374ac916b94376e863fb8724`  
		Last Modified: Tue, 11 Jul 2023 00:37:00 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f329fb50eacdf8129b913448f5455fd7152aaa79500767dfa760b694da73feb`  
		Last Modified: Tue, 11 Jul 2023 02:10:36 GMT  
		Size: 2.4 MB (2425334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2002da5c191691ff7fed00a89021e983f726e4a60326ba8beae7f95e428580`  
		Last Modified: Tue, 11 Jul 2023 02:10:35 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a19c37d591445b932ec4166f5a0ab16aff77d86a7f2a1dcade9e055a3d0a0f`  
		Last Modified: Tue, 11 Jul 2023 02:10:36 GMT  
		Size: 698.2 KB (698235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa944465ea81f50d6d32c444e4f9f38705abfee129135c3c7e5636ced0b23831`  
		Last Modified: Thu, 03 Aug 2023 00:52:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc2221aa2563b440cd1b2cd372bf1513db899ebe5a7286dff781be7ea111cd`  
		Last Modified: Thu, 03 Aug 2023 00:52:48 GMT  
		Size: 18.5 MB (18506942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; ppc64le

```console
$ docker pull drupal@sha256:e97fdf9a2f3c50de99fc402e8d8bec58d0dc5b8ae25831aff2c2bbe7d4452b5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55498025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21216b26a9d7a0132ed599d1d63128fb23a377a07ed2e6b9385970632b5c2b3e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 02:20:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 02:20:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 02:20:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 02:20:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 02:20:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 02:20:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 02:20:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 02:20:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 03:11:20 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 23:06:18 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 23:06:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 23:06:19 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 23:06:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Aug 2023 23:06:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:14:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 23:14:26 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:14:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 23:14:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 23:14:28 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 23:14:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 04 Aug 2023 23:14:31 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Aug 2023 23:14:31 GMT
EXPOSE 9000
# Fri, 04 Aug 2023 23:14:32 GMT
CMD ["php-fpm"]
# Sat, 05 Aug 2023 00:33:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 05 Aug 2023 00:33:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:33:40 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Sat, 05 Aug 2023 00:33:40 GMT
ENV DRUPAL_VERSION=10.1.2
# Sat, 05 Aug 2023 00:33:41 GMT
WORKDIR /opt/drupal
# Sat, 05 Aug 2023 00:34:08 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 05 Aug 2023 00:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a82af153dde64aaecebbaa654ef25fe458cadc53b82b53ef2709b36ee12472`  
		Last Modified: Thu, 15 Jun 2023 04:11:27 GMT  
		Size: 2.7 MB (2743785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513a439724cb0dce6489fcef92ec4c613854488cc971907f16b38f06ff6e8a14`  
		Last Modified: Thu, 15 Jun 2023 04:11:26 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c5f3fdb07b83b724766e77b9ffeaaa86c0112dc077280c28d8ab36d1b52955`  
		Last Modified: Thu, 15 Jun 2023 04:11:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e43e434ad997a9a719b15871b8f74f51c962cdc854a377cf34fa39200eba479`  
		Last Modified: Sat, 05 Aug 2023 00:04:07 GMT  
		Size: 11.8 MB (11829761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b68142c845ef53e1e64a4aec650de4ad8174d4aacdd4cecec4551774756726a`  
		Last Modified: Sat, 05 Aug 2023 00:04:06 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac2f2b84e5d11ca0e6bada92ebfeec7a2cb7c75282962476b7666437353606`  
		Last Modified: Sat, 05 Aug 2023 00:04:51 GMT  
		Size: 16.1 MB (16092607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4763046370bd5372f9529b6d051b1ac1670e11ddc2c2cd905177807d709ab`  
		Last Modified: Sat, 05 Aug 2023 00:04:46 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce78ae4e2ecd2374c3a17acc330c0163b9763efcccb39644c75ad930ef561fc4`  
		Last Modified: Sat, 05 Aug 2023 00:04:47 GMT  
		Size: 18.8 KB (18781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22241fa72cbd0a8f8a7061c197b6ecf279de2003f8b900cd42b6cfd1dfd1cb13`  
		Last Modified: Sat, 05 Aug 2023 00:04:46 GMT  
		Size: 8.9 KB (8885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831cc241c010d9c07323073b849b21acd800dc11508a434c700b76fd96f1e04a`  
		Last Modified: Sat, 05 Aug 2023 00:57:12 GMT  
		Size: 2.2 MB (2249079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a8a94deff4060472011d4c16a48d72fba116fb7d0027ca45a279588adb8632`  
		Last Modified: Sat, 05 Aug 2023 00:57:11 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f8fa6a7c4a7b153aa0e14b164a06fb80ff372f2e8f73f5c9d83281a3c9892a`  
		Last Modified: Sat, 05 Aug 2023 00:57:12 GMT  
		Size: 698.2 KB (698238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c5f897fe97b929dd9ee2d28ab2c0af7bdc8ede3e6c8b291207b935b1475b31`  
		Last Modified: Sat, 05 Aug 2023 00:57:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456e90ec192e77450252db59b09b5982315bd37bb095f9e485717a296db67fb`  
		Last Modified: Sat, 05 Aug 2023 00:57:35 GMT  
		Size: 18.5 MB (18507166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.1-fpm-alpine` - linux; s390x

```console
$ docker pull drupal@sha256:505a2b14115628de7d9259f74fcbd062195cd34d7298a0cb4b989ce39127ca15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53861895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f9ad3e301ab58e41cf1ed4e7e8b4566194389c343c486cd78c208b02477b990`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 18:32:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 18:32:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 18:32:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 18:32:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 18:32:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 18:32:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 18:32:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 18:32:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 19:47:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:46:22 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:46:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:46:22 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:46:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Aug 2023 22:46:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:51:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:51:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:51:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:51:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:51:46 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:51:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 04 Aug 2023 22:51:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Aug 2023 22:51:47 GMT
EXPOSE 9000
# Fri, 04 Aug 2023 22:51:47 GMT
CMD ["php-fpm"]
# Sat, 05 Aug 2023 00:31:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 05 Aug 2023 00:31:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:31:15 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Sat, 05 Aug 2023 00:31:16 GMT
ENV DRUPAL_VERSION=10.1.2
# Sat, 05 Aug 2023 00:31:16 GMT
WORKDIR /opt/drupal
# Sat, 05 Aug 2023 00:31:26 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 05 Aug 2023 00:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9863b5dcc3e5885fe5ff8335b86d4287dfd59b451fe22e94b79f83b396c3776d`  
		Last Modified: Thu, 15 Jun 2023 21:54:07 GMT  
		Size: 2.8 MB (2766871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f159305449b6c309659dadfedb968259be79e6f5b9f552d97134f0a94490ae8`  
		Last Modified: Thu, 15 Jun 2023 21:54:07 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e5f78cdbb2bcfe6b24c6cc002d51d1551a0fbabd06fa3baaee2be566d6d55f`  
		Last Modified: Thu, 15 Jun 2023 21:54:07 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91426ebd6d39b611931e44a363124a185ab3c4342d886cad7d03a43ee8925b7`  
		Last Modified: Fri, 04 Aug 2023 23:23:13 GMT  
		Size: 11.8 MB (11829761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08ebbf62532d3616c6f7f55a731b5a97797cb24a661a95a7cfa624fbfe5c4c8`  
		Last Modified: Fri, 04 Aug 2023 23:23:11 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945ac6aa727eff35a4a3bad29c57d29f59ed00f421fa61d036574ef95d04bdf9`  
		Last Modified: Fri, 04 Aug 2023 23:23:30 GMT  
		Size: 14.8 MB (14823826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30fecf4e5ea32728261050b2fecc53f6417fffd6bddbba06a93eba80a7bd376`  
		Last Modified: Fri, 04 Aug 2023 23:23:28 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89086795fc457d5fee1ffc174485949b7c5cf052afd3f469041e1dd405771c5e`  
		Last Modified: Fri, 04 Aug 2023 23:23:28 GMT  
		Size: 18.8 KB (18798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b409195fdce6486a6aec3f65d4438b7efa231b7bf8cead90bb75439029090158`  
		Last Modified: Fri, 04 Aug 2023 23:23:28 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ded5c4bc6bf8eab162e53a9cfb188429137a1e26f6d94703c39c10c5b3d6614`  
		Last Modified: Sat, 05 Aug 2023 00:44:51 GMT  
		Size: 2.0 MB (1990106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a267d0670bb8cfe56ad8762971127d1d89a1433e8d9e82328068292409723267`  
		Last Modified: Sat, 05 Aug 2023 00:44:50 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f650c09693dd777c29d7b3248804fd66670348a3c7e1424fab78450987d4d7`  
		Last Modified: Sat, 05 Aug 2023 00:44:50 GMT  
		Size: 698.2 KB (698236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4a308dfab0f3d1fd6de6e5438204ec018a16eb17f745faaeecf1c6fd2ac4ad`  
		Last Modified: Sat, 05 Aug 2023 00:44:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb9bd5110aa34190b01456569655a9090aaf27de7ca5945cefe761d043a8ed0`  
		Last Modified: Sat, 05 Aug 2023 00:44:54 GMT  
		Size: 18.5 MB (18506982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
