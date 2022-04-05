## `drupal:rc-php8.1-fpm-alpine3.14`

```console
$ docker pull drupal@sha256:0dad30077e1ecc2aafd05c0fe6bc8ad384f28c55c998420f3002ec10bd0333d4
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

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; amd64

```console
$ docker pull drupal@sha256:5dfd00e9510f4e6ae496c960bbe857ebaad768ead3e73baa2dbecca79e8a8196
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50749257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ca7c0a7eb88fd3ff9c5bb56a6920fd4a54b7c22f70741fd5331067a73e197f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:11:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 01:11:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 01:11:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 01:11:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 01:11:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 01:11:41 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 01:36:03 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 01:36:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 01:36:03 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 01:36:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:36:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:47:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:47:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:47:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:47:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:47:57 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:47:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:47:58 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:47:58 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:47:58 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:44:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:44:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:44:25 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:44:25 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Tue, 05 Apr 2022 11:44:25 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:44:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:44:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa03774f3e03c326f200279ce7ca2ddf335bd09a519355bf8a0dbf95e5491caa`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 1.7 MB (1703109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaafb366c9f65869a27c1ae891cf1a8b9fb9be95a65f7d733b5bd38dcad8b9a`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7627ccdb679dac7fbcd955eed5f3c213f86c69ffd5ce9d0316d3af984a2bd0`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e41c7b921a8d1068466c7ad13952b59860746c3eac719d7d546d1865c1215b`  
		Last Modified: Tue, 05 Apr 2022 02:51:58 GMT  
		Size: 11.7 MB (11720122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9a86762fb65afbd1cfa9332e0e3729242f0a4930dfb1bee4910453823b7d5`  
		Last Modified: Tue, 05 Apr 2022 02:51:57 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921563ee8ef8c220342ed41b3887bc05e87e1a19073ad4f680275c2984c0252c`  
		Last Modified: Tue, 05 Apr 2022 02:52:28 GMT  
		Size: 12.3 MB (12325105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab2dd3298a84f47a05efd548d093fac21450e395ea9340cd9d24d4efcaf7db5`  
		Last Modified: Tue, 05 Apr 2022 02:52:26 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a20083ff645c51d15d9789b8463356b5725a80f5f1461b953c76f3eac87bdb`  
		Last Modified: Tue, 05 Apr 2022 02:52:26 GMT  
		Size: 18.5 KB (18520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6446000618a2227fe19c1666f74ec1f6f1bca1fb03c4d07d237c743027732e`  
		Last Modified: Tue, 05 Apr 2022 02:52:26 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33733486b02b0c73b90d293b167e13cd5ba1399bf17fb239d1656f4d247e06bb`  
		Last Modified: Tue, 05 Apr 2022 11:55:57 GMT  
		Size: 2.4 MB (2361102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dde9c9a5d37128f425201a40cfb703e76a8dfa74c09f68eb55df23bb457c47e`  
		Last Modified: Tue, 05 Apr 2022 11:55:57 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef81e871ba556e3d5e624a835d5c8dcf34b3cfda228b3d234a8d2644743c21c`  
		Last Modified: Tue, 05 Apr 2022 11:55:57 GMT  
		Size: 660.1 KB (660093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94351deca7dd7931f8d2c37423bbab6db6963ab364a6caf9b2f15ea51b4b0ef5`  
		Last Modified: Tue, 05 Apr 2022 11:55:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e665f74e3499a85ddadf04a276d65ce5b45be832f5bdd12d66a49c1bac7c359`  
		Last Modified: Tue, 05 Apr 2022 11:56:01 GMT  
		Size: 19.1 MB (19129274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; arm variant v6

```console
$ docker pull drupal@sha256:2df1c061c4dd7e83f89699cace83f63a691db9f165cd62c7f4d4c247fb108b83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48905180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7ab3a5a205cb9923bfacdaa104bf9710654ef40e0e583d55d72db6ea4d1026`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 01:03:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 01:03:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 01:03:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 01:03:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:03:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:03:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:03:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:03:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:03:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 01:03:10 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 01:03:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 01:03:11 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 01:03:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 01:03:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:12:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:12:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:12:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:12:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:12:40 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:12:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 01:12:42 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 01:12:42 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 01:12:43 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 02:58:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 02:58:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:10:21 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:10:22 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Mon, 04 Apr 2022 21:10:22 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:10:52 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:10:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68acfb8e127d2000623a5b46b3ad33f9390aa70683d5a7e3ac3953342ab3d3d`  
		Last Modified: Tue, 29 Mar 2022 02:11:05 GMT  
		Size: 1.7 MB (1691160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361518c45781f43fe4762fce5917a961584d0ecc89203bafe481dfada1d0ae1`  
		Last Modified: Tue, 29 Mar 2022 02:11:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d1e46eaa8bdfc75786427e73b0f17121c1a7d669842d21e2b4d9bf0915ff29`  
		Last Modified: Tue, 29 Mar 2022 02:11:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a36496ee2bcb40459c1ccfd3cd7d3034658bd2ef557d222f463bafb4285a7d2`  
		Last Modified: Tue, 29 Mar 2022 02:11:05 GMT  
		Size: 11.7 MB (11720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43fca19db03a92a856472bde8e604499829450ec97bd100969bc8ba1ad5cff6e`  
		Last Modified: Tue, 29 Mar 2022 02:11:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df249806464529493339718cc56e1a5fe82f7afc2a4802168f8ef3d306b6aef9`  
		Last Modified: Tue, 29 Mar 2022 02:11:58 GMT  
		Size: 11.2 MB (11220107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e02841a5d6cf5992b76675d7cfb6dc7878d75995dbd2dd7ea2059d3ab6b9fa`  
		Last Modified: Tue, 29 Mar 2022 02:11:49 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feb69db800fcfb8835dba0f2a55ea2581cd98a9715aae4ef2cdad982aba4068`  
		Last Modified: Tue, 29 Mar 2022 02:11:49 GMT  
		Size: 18.3 KB (18340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc6fc08344b50d03780a0164aa3b8d67aec2535544645a7546b2a8970a6f135`  
		Last Modified: Tue, 29 Mar 2022 02:11:49 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d39cd6c463ec9ecb8be856815b17a1a121ded29159709598be66471d4c3b1`  
		Last Modified: Tue, 29 Mar 2022 03:19:20 GMT  
		Size: 1.8 MB (1826453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f414d6d1fb67d78d869f92784e704a906be376eb7450426146a703bb1e7d42a7`  
		Last Modified: Tue, 29 Mar 2022 03:19:19 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fd1db82675bbd7b2ae216ec504f719fd8a9b053b6e3a134c921ad8f64d569a`  
		Last Modified: Mon, 04 Apr 2022 21:24:38 GMT  
		Size: 660.1 KB (660098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd7bb27c6ed584576f2d050839acefa267c38ee7c2ee9df6aa71a95414a1c1b`  
		Last Modified: Mon, 04 Apr 2022 21:24:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca21c923a905d8430b37e7658d65437151e95a95e17f4a95eee603e0be22620`  
		Last Modified: Mon, 04 Apr 2022 21:25:05 GMT  
		Size: 19.1 MB (19129324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; arm variant v7

```console
$ docker pull drupal@sha256:fb29cdab987bb75d06ebc80bb1bf283abf2011d598da5607939d044b36de2cd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47746217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18cbc2f107d1c092544d0f5a8c9d327d23595b4985c2bd54e593801e6cad615a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:41:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 07:41:52 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 07:41:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 07:41:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 07:41:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 07:41:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:41:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:41:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 07:41:58 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 07:41:59 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 07:41:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 07:42:00 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 07:42:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 07:42:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:51:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 07:51:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 07:51:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 07:51:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 07:51:17 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 07:51:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 07:51:19 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 07:51:19 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 07:51:20 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 11:19:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 11:19:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:31:20 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:31:20 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Mon, 04 Apr 2022 21:31:20 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:31:52 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:31:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d54f9e882a75e957680bbb788bf5a094e6a788d69b093f489fef69498cf6f7`  
		Last Modified: Tue, 29 Mar 2022 10:38:06 GMT  
		Size: 1.6 MB (1558928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac5ce9becbc99b4ca9ab350939bdb94a5657465e688f0d4e6413d07d0454a27`  
		Last Modified: Tue, 29 Mar 2022 10:38:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430efedf2eda2718b96667efdf683a05edad9eeae68dae93431bd6d008ef291`  
		Last Modified: Tue, 29 Mar 2022 10:38:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d63ce9fafc9619919431fce39030e38d3c58c23caf02539079e94e41b1360f`  
		Last Modified: Tue, 29 Mar 2022 10:38:06 GMT  
		Size: 11.7 MB (11720135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d83e3cc50bbd873791884f024fb6afd367fc8687d0f8d2ade600ab407dda26d`  
		Last Modified: Tue, 29 Mar 2022 10:38:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ebd36c0219e5e9909c191319fe88740e5437041d62102e945e488584a1d9d6`  
		Last Modified: Tue, 29 Mar 2022 10:38:53 GMT  
		Size: 10.5 MB (10541523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7612480bc05709e72b5aa1c605132636fa86dec17d6a7b068268e618b576ee`  
		Last Modified: Tue, 29 Mar 2022 10:38:49 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95960c8399608056c188c940ae49d4515a6211edd251f638e93e2d450513d81e`  
		Last Modified: Tue, 29 Mar 2022 10:38:49 GMT  
		Size: 18.3 KB (18317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306350e11bd787625bbaf57eab1c263cd4058faf8858b83ca55c4ba4c2733c16`  
		Last Modified: Tue, 29 Mar 2022 10:38:49 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005a8997f90bd1792701584ab4cc5b1118dabe097b7926e152ae4acb2fcd6708`  
		Last Modified: Tue, 29 Mar 2022 12:27:56 GMT  
		Size: 1.7 MB (1676395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1e3acdd5963faaa49cfe9d987c6d314e9b26113e8193a1b5d43ed35aaeb683`  
		Last Modified: Tue, 29 Mar 2022 12:27:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a383c1fccc0a648e282ac39e1a8d07246ca1b856a83c86f73f16424e0c145599`  
		Last Modified: Mon, 04 Apr 2022 22:15:13 GMT  
		Size: 660.1 KB (660097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd0c5bb45ae128e1f47e47b984e9790bb30188ee6e2a10bede21a84aaf0bd95`  
		Last Modified: Mon, 04 Apr 2022 22:15:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253556e60c1ed7e19f121ac1edc3a7ed289002a5bbdad63f58924cedde2283ff`  
		Last Modified: Mon, 04 Apr 2022 22:15:41 GMT  
		Size: 19.1 MB (19129299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:d6c2087bf96f79bf48968d0b9be4863f9da2d5f16a67007d8cac206987a7435e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50960383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68997772b7baff0b46de7c452beadc121d41e0dd9401a8539fd92a3d7f8dcad6`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:55:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:55:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:55:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:55:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:55:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:55:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:55:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:55:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:55:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 02:55:26 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 02:55:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 02:55:28 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 02:55:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 02:55:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:15:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:15:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:15:26 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:15:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:15:28 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:15:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 03:15:30 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 03:15:31 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 03:15:32 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 15:17:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 15:17:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:20:56 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:20:56 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Mon, 04 Apr 2022 21:20:57 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:21:10 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:21:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d23547051480ea2370b812b539a9689be31bd4f8da8c77cb7dae8567c362e2a`  
		Last Modified: Tue, 29 Mar 2022 05:35:38 GMT  
		Size: 1.7 MB (1699722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94519d769f58083ef844d873bb3dad0e202820cd05de9326b4d6f0e555af95d6`  
		Last Modified: Tue, 29 Mar 2022 05:35:36 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d175b6b77a31ce89a09c5ac0f84caca9af0c8f17c6ee598cf3d506a6f2af6a11`  
		Last Modified: Tue, 29 Mar 2022 05:35:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a25522f37799ac0abf550ceaa7d55fa219268ee5f84eb6f08076b372256926`  
		Last Modified: Tue, 29 Mar 2022 05:35:35 GMT  
		Size: 11.7 MB (11719978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8243227c8b91f3ec39bf39a2e798c66c86567ade7c009b68525cf9efbb5c2f87`  
		Last Modified: Tue, 29 Mar 2022 05:35:34 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a6bb189c052936bada28edd48cc339ddc1951b179492e3f361b08a86e5670`  
		Last Modified: Tue, 29 Mar 2022 05:36:10 GMT  
		Size: 12.4 MB (12392972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d9b6e92e1a4ebb02c364f252b373ca8821584292f485161f56cabe55755a94`  
		Last Modified: Tue, 29 Mar 2022 05:36:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9931519e7fcd0969b76fa6561f25e21517e9ce927db32a263f144419fb077a21`  
		Last Modified: Tue, 29 Mar 2022 05:36:08 GMT  
		Size: 18.3 KB (18259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7344bc2485443a8b51a051176f590d1120bbf09b6c2b29a4db533e3796939440`  
		Last Modified: Tue, 29 Mar 2022 05:36:08 GMT  
		Size: 8.6 KB (8623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14521d3766b910998462f9933f4e27f22162b6cbb85d7340b8ecaeffd2623347`  
		Last Modified: Wed, 30 Mar 2022 15:48:08 GMT  
		Size: 2.6 MB (2608870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d08d1151de7acaf1761e5f1f35576a449f16d648d189c130e2908bc033ea76`  
		Last Modified: Wed, 30 Mar 2022 15:48:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19134089d40d986cc239064ecaf513afb2914f3ca691c76cddf3bc3138789648`  
		Last Modified: Mon, 04 Apr 2022 21:42:17 GMT  
		Size: 660.1 KB (660107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af588501ccf937271c2c405c8dfcb55c18ec59ea033316782b4b7963c4598f3c`  
		Last Modified: Mon, 04 Apr 2022 21:42:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8727e068429b32079150c3f5e18b62af3d51737297ec7084b6bf5d60b88ce`  
		Last Modified: Mon, 04 Apr 2022 21:42:23 GMT  
		Size: 19.1 MB (19129519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; 386

```console
$ docker pull drupal@sha256:c5dd804854d227190f7745fb08eddf09a2efef22c3e118e9d7c932fc2b63cffd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51250197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d990f8a7ad654c1332676077dad307836bdf7d484b05f12fca76c52b01754b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:13:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:13:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:13:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:13:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:13:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:13:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:13:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:13:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:13:37 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:29:37 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:29:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:29:39 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:29:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:29:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:36:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:36:43 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:36:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:36:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:36:45 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:36:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:36:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:36:48 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:36:49 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 07:36:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 07:36:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 07:37:01 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:37:01 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Tue, 05 Apr 2022 07:37:02 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 07:37:15 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 07:37:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d252c7fc7fdf2acebba22bdce0df2a9b6699d3103f77cd3befcd96c9830dd44d`  
		Last Modified: Tue, 05 Apr 2022 01:25:00 GMT  
		Size: 1.8 MB (1801196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29da06ea807d8f1d3f704ed6147c9f34dbf3dd2c26817a9f8b1ee7643d57a281`  
		Last Modified: Tue, 05 Apr 2022 01:24:59 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9b1421b6c940a062a92e05e3ac5394ef9dc0292558b91f73f4d1ced04a14`  
		Last Modified: Tue, 05 Apr 2022 01:24:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd8c2922dd19809b6db1de520a0f923542ea8bcbadd0041e58f23d7d34ae272`  
		Last Modified: Tue, 05 Apr 2022 01:27:59 GMT  
		Size: 11.7 MB (11719957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80654e2534edb8975a0fa4025378b5418775913282166e076398cc8c3b588700`  
		Last Modified: Tue, 05 Apr 2022 01:27:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84f2903dc7fd835ddda05f3a5e6cd95466995734f56c7945936525f61361a89`  
		Last Modified: Tue, 05 Apr 2022 01:28:38 GMT  
		Size: 12.6 MB (12611327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef42808a8fa9fc4432c201396604816e44d6bb3e4e04c2d1ecb53f9350365966`  
		Last Modified: Tue, 05 Apr 2022 01:28:36 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e66c292a1d01ccb45e4deaf4dee2056812c92914771260f6820294e9fa2341`  
		Last Modified: Tue, 05 Apr 2022 01:28:36 GMT  
		Size: 18.4 KB (18419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e64c814a1ad005b896da6cba3cdf543688e59439784fec4bd43deafdfde9cf`  
		Last Modified: Tue, 05 Apr 2022 01:28:36 GMT  
		Size: 8.6 KB (8618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca49d314f97953cc1ddc2b7de41b4e22ee5a262c8737b314dca152c3d0901a4`  
		Last Modified: Tue, 05 Apr 2022 07:55:04 GMT  
		Size: 2.5 MB (2475646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4672322ee8569bd418c62468fcbde9f05ba02c9fc5bb410c19ca036cfb4c18`  
		Last Modified: Tue, 05 Apr 2022 07:55:04 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4203904cc7ec95356e43798fb56370d021273bb49653ce72faddcd92a9286a3d`  
		Last Modified: Tue, 05 Apr 2022 07:55:04 GMT  
		Size: 660.1 KB (660089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e448bc943b1cdfd0aa014ab76c6a501a266034e6d7eed4165997e751dcd021`  
		Last Modified: Tue, 05 Apr 2022 07:55:03 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07393e152888e28aa202e4b7c48829844b027822100d4cb614bf643a86bae68`  
		Last Modified: Tue, 05 Apr 2022 07:55:08 GMT  
		Size: 19.1 MB (19128903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; ppc64le

```console
$ docker pull drupal@sha256:182529e12e7cda5ccc496c154455d87d66b6eb32ffd0d65365ff87ca7def3c37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50946114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63307d0a00d6a98b43d3e71732856458944f34870183998d56f5290adb548bdd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:24:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:24:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:24:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:24:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:24:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:24:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:25:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Mar 2022 02:25:03 GMT
ENV PHP_VERSION=8.1.4
# Tue, 29 Mar 2022 02:25:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 29 Mar 2022 02:25:10 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 29 Mar 2022 02:25:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 02:25:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:35:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 02:35:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:36:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 02:36:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 02:36:16 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 02:36:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 02:36:27 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 02:36:30 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 02:36:33 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 18:05:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 18:06:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 22:08:18 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 22:08:22 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Mon, 04 Apr 2022 22:08:24 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 22:09:03 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 22:09:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac47bb21f777673b7d46d5ae2af561e7ee41f8e704fac1c95c7092705ff71575`  
		Last Modified: Tue, 29 Mar 2022 05:12:48 GMT  
		Size: 1.7 MB (1748184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763b14c5a184a7da21176d18945d140cb7780e4172dbd04171773c21aec7c462`  
		Last Modified: Tue, 29 Mar 2022 05:12:47 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61e5e97d5a4e8eaa92a458a712cf3deb2c7c2316ef376cd1ee5a8c113cf6cf8`  
		Last Modified: Tue, 29 Mar 2022 05:12:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fd04fbda6ad743e2c40b38e3a784a9bea6dfc3dafc4f2fb1d1ee75dca4288`  
		Last Modified: Tue, 29 Mar 2022 05:12:46 GMT  
		Size: 11.7 MB (11720163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d85c946f914b49929cffcaff04d10b4610c12b697a923373b8e73bc013187a`  
		Last Modified: Tue, 29 Mar 2022 05:12:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f97811bbef6cc8b5de1f112a44f2409b57636c1f1a5dab314bc24b4a506522`  
		Last Modified: Tue, 29 Mar 2022 05:13:26 GMT  
		Size: 12.7 MB (12721017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509951b1d92975cc5977b322531f8f1072ca2f664d572913426d5feb46037233`  
		Last Modified: Tue, 29 Mar 2022 05:13:23 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad4d1bf324bdbdd823b43ef8390406b627dd6e6161f9f02ee149860b0a401a9`  
		Last Modified: Tue, 29 Mar 2022 05:13:23 GMT  
		Size: 18.3 KB (18340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991e70328e013aa72ebe3a43dde3e9090206fed033823e213f8c391c4274430c`  
		Last Modified: Tue, 29 Mar 2022 05:13:23 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09a4be50677c44bd06eb25553780aafccd76632a2a6e86ea8432f0154182e5d`  
		Last Modified: Wed, 30 Mar 2022 19:47:20 GMT  
		Size: 2.1 MB (2121141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca374296037888111289b831ee018f03a08fba948db5c99a7fcf13cc44172a7b`  
		Last Modified: Wed, 30 Mar 2022 19:47:17 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49374b2a0c8813dbdc5a60a8bb92556fe7a8e04ea307092276b0239e281e8e9e`  
		Last Modified: Mon, 04 Apr 2022 22:53:19 GMT  
		Size: 660.1 KB (660101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306a96f6bbc689fc6b4e54bc419341e4915a615ee04c742a81633dcffcfefe96`  
		Last Modified: Mon, 04 Apr 2022 22:53:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9a0bb9aae64e0fe7b6cf2193d360ddeaa161511059f56ab191fa1a33432c6`  
		Last Modified: Mon, 04 Apr 2022 22:54:59 GMT  
		Size: 19.1 MB (19129406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:rc-php8.1-fpm-alpine3.14` - linux; s390x

```console
$ docker pull drupal@sha256:6e68a94a6a3282c8fac9cd55cb082292ab2b08a56513ff874e8ab569e8181330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49441947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0bc2a5de72b6a37b0720e7ed8d288e684f1d58c27c0ccaed4e0e52a0db2ac02`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:08:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:08:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:08:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:08:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:08:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:08:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:08:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:08:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:22:06 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:22:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:22:06 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:22:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:22:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:27:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:27:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:27:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:27:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:27:56 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:27:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:27:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:27:57 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:27:57 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:48:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:48:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:48:12 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:48:12 GMT
ENV DRUPAL_VERSION=10.0.0-alpha2
# Tue, 05 Apr 2022 11:48:12 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:48:25 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:48:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2af9291e8bb0cd2e6ac744794ab2287652d0f0e3b0a1e03feba1ccf6cdc9ef0`  
		Last Modified: Tue, 05 Apr 2022 01:10:11 GMT  
		Size: 1.8 MB (1762717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6e28b72f7a6dc4fe85e004996700ffc40c5583e3c5b6dc6561c829ac179b2`  
		Last Modified: Tue, 05 Apr 2022 01:10:10 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a6f63d4dae3713973596b3706bfaa082a0232b19dfb450921a282b03776550`  
		Last Modified: Tue, 05 Apr 2022 01:10:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714961eb5c30e62c9e7cd5344846e287e3c1b13e692212e86c7a4e73a1c4f129`  
		Last Modified: Tue, 05 Apr 2022 02:52:32 GMT  
		Size: 11.7 MB (11720146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c082dae5f26fd99fcdb448b9f31b0b708a5079d33308eed683f6b1d1602bb7c9`  
		Last Modified: Tue, 05 Apr 2022 02:52:32 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432986b119778a90ead2e1a30674d72c92439e2f70a5b3f8d840631eb987f505`  
		Last Modified: Tue, 05 Apr 2022 02:52:55 GMT  
		Size: 11.5 MB (11530714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cedb0eb43bf737008c7c7cad174fa7a78bbb0847721fe212af23e6796b7a007`  
		Last Modified: Tue, 05 Apr 2022 02:52:53 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36bab6a34757ddbdfb1716e9e871a365e0d04af9fa9b171ca43547303e41668`  
		Last Modified: Tue, 05 Apr 2022 02:52:53 GMT  
		Size: 18.4 KB (18367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed507e81855b0708defd7ba2874bdf6330b6ef763ecfc4270d43fae13c262219`  
		Last Modified: Tue, 05 Apr 2022 02:52:53 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4afba2408f1f7e8b966c5ff893a1b954c7643e5c64e277e0c8e65ae270a931`  
		Last Modified: Tue, 05 Apr 2022 12:06:32 GMT  
		Size: 2.0 MB (2003149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a893ec7730787579408a1d80e29e9e5e72e8772a325bfcc41a694ad71f2bc2`  
		Last Modified: Tue, 05 Apr 2022 12:06:32 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f06a773cee3d7f29b2d5b06ad78eda56703592106fa534b25f22c5fedad5a4`  
		Last Modified: Tue, 05 Apr 2022 12:06:32 GMT  
		Size: 660.1 KB (660096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e7711352c7e9efc6e0383a26f3aaa73805ec043e28b05c38a7c605a1907515`  
		Last Modified: Tue, 05 Apr 2022 12:06:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9252e0e03c8e380f21e84fb8de876c35feb14639b72c0ffd3995308c9a6b8df4`  
		Last Modified: Tue, 05 Apr 2022 12:06:36 GMT  
		Size: 19.1 MB (19129117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
