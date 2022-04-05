## `drupal:9-fpm-alpine3.14`

```console
$ docker pull drupal@sha256:e6c08d0f1f05b16fd4ab6655623a5b9fc9a4aa6e3ede34783e0790dd215bb0b2
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

### `drupal:9-fpm-alpine3.14` - linux; amd64

```console
$ docker pull drupal@sha256:3b16e32fc8d39b956aa18946ec0058a4cb4ea858b732614216cf8c02a134424d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51490968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7b58731f4617556b92ee6d146d003a6f41aa1031640d37cfdad1b508e4e8e4`
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
# Tue, 05 Apr 2022 02:00:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 05 Apr 2022 02:00:07 GMT
ENV PHP_VERSION=8.0.17
# Tue, 05 Apr 2022 02:00:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 05 Apr 2022 02:00:07 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 05 Apr 2022 02:00:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 02:00:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:11:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 02:11:31 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:11:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 02:11:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 02:11:33 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 02:11:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 02:11:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 02:11:33 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 02:11:34 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:47:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:47:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:47:41 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:47:42 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 11:47:42 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:47:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:47:56 GMT
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
	-	`sha256:c26d525a4988d246701deb9916c4ff3ed1391d0960a696c4a2ebf06aa12872ba`  
		Last Modified: Tue, 05 Apr 2022 02:53:41 GMT  
		Size: 10.8 MB (10790927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7cd4551d5b0f66e4b4cb6880fddb181a5315688303ac7df086586aefe93c29`  
		Last Modified: Tue, 05 Apr 2022 02:53:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a513af0a01122a462e254e6d6bbcd5467afbb391acdeb2935b862a6222f08136`  
		Last Modified: Tue, 05 Apr 2022 02:54:00 GMT  
		Size: 12.0 MB (12031327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e98a34b92f3960de1c3e37c340ec0cc7c6be8e598f3e6de80a877c550e271f7`  
		Last Modified: Tue, 05 Apr 2022 02:53:58 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba84251fbafbccff2c1220b11f2c1467519c03549da7c654a2bb8c5f3d79a36`  
		Last Modified: Tue, 05 Apr 2022 02:53:58 GMT  
		Size: 18.3 KB (18328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b5520cc01040c3a529c06a9e88a3e2027dfbefecb6f8ecd70e311c1c2eb556`  
		Last Modified: Tue, 05 Apr 2022 02:53:58 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d289363fdcbda00d7b2f2dbf5aa394a5a93bcfae17f69571b617b38dbdacad`  
		Last Modified: Tue, 05 Apr 2022 11:57:34 GMT  
		Size: 2.5 MB (2517916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abaabef8ca0cc1d32975149a7cfcd6b151474d5e771d629ae0fd0d7c25cfe05`  
		Last Modified: Tue, 05 Apr 2022 11:57:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f4700597bd198d466b2da8a49329f6f4c10ccab9166ff84b2bdc1d09a52898`  
		Last Modified: Tue, 05 Apr 2022 11:57:34 GMT  
		Size: 660.1 KB (660095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da869445ea82cc8b628c2026422be095fd25fcfcced67a46f034a2713645172`  
		Last Modified: Tue, 05 Apr 2022 11:57:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4f894fee60543d913307ec11daa25ae19d2406adf0351264eb2b453316ef65`  
		Last Modified: Tue, 05 Apr 2022 11:57:38 GMT  
		Size: 20.9 MB (20937379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; arm variant v6

```console
$ docker pull drupal@sha256:4d4385603a3d4b3b0569a543ce46afdcf943cc358cf0eec33ff6084b72f56081
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49700783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3853b54d40f959189f8e65867415c9c16be1d5659e1b874d2c578dbbe629901`
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
# Tue, 29 Mar 2022 01:23:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 01:23:01 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 01:23:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 01:23:02 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 01:23:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 01:23:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:32:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:32:26 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:32:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:32:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:32:29 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:32:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 01:32:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 01:32:32 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 01:32:32 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 03:03:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 03:03:23 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:12:13 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:12:14 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:12:14 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:12:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:12:46 GMT
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
	-	`sha256:9789f21a4d69d632875154a60f5a8ad0e01c4145d1376d312b6f11dbdf00c229`  
		Last Modified: Tue, 29 Mar 2022 02:13:29 GMT  
		Size: 10.8 MB (10790939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e8169f20755fe04c920ec00cb16e341361c20d96999379c13afc33a9a3f8f`  
		Last Modified: Tue, 29 Mar 2022 02:13:26 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3825fa8fd288f2c4063b6b3c069e1761045d956a297d7ad2cf88e5072bf551d5`  
		Last Modified: Tue, 29 Mar 2022 02:14:04 GMT  
		Size: 11.0 MB (10966991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae69e64e85331658df110108b5a07a6e4c58b8a9e878711c0b1e60e98cd4b4d1`  
		Last Modified: Tue, 29 Mar 2022 02:13:56 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892a0b1aed793ee1721e19ab3612fce595180c26e5c395cf03d040cb9430c0ea`  
		Last Modified: Tue, 29 Mar 2022 02:13:56 GMT  
		Size: 18.3 KB (18340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d826db64949c608c646ea6d01171c42fbd2794c0e0aec4ed47f6acdf07761189`  
		Last Modified: Tue, 29 Mar 2022 02:13:56 GMT  
		Size: 8.6 KB (8567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208b8a28a1c9eb3cc4c69cc77b8f976d3c1f4524d6f17071b73f07446ac599cf`  
		Last Modified: Tue, 29 Mar 2022 03:21:33 GMT  
		Size: 2.0 MB (1995913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab86a56c22aa477d8a079a9753914517e7f3f3d5234cc1ecc62ef8d0d6a5499c`  
		Last Modified: Tue, 29 Mar 2022 03:21:32 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3550b1de2acc51b72760776f4570e514a5caa90164e3c9ce588a4a4e3075730`  
		Last Modified: Mon, 04 Apr 2022 21:27:03 GMT  
		Size: 660.1 KB (660101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfc07af5328f679911cf5643a652f954f2ed99903cc681e00ae1226dd7af5f1`  
		Last Modified: Mon, 04 Apr 2022 21:27:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed04ca5bdb1b26ad5005e0b2593971df61f2d45914f8f48c7331f41f72761e8`  
		Last Modified: Mon, 04 Apr 2022 21:27:32 GMT  
		Size: 20.9 MB (20937816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; arm variant v7

```console
$ docker pull drupal@sha256:f68e13d5180badcaa1251ba586f1f246980ed0f9255dcdca53b5eab5f20ec2ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48551349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0b2d7afc443128291d857ef7b75c15dca74073c7d0f2e445b39c049a15b85b1`
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
# Tue, 29 Mar 2022 08:41:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 08:41:30 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 08:41:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 08:41:31 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 08:41:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 08:41:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:50:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 08:50:41 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:50:44 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 08:50:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 08:50:45 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 08:50:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 08:50:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 08:50:47 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 08:50:48 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 11:37:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 11:37:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:37:13 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:37:14 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:37:14 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:37:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:37:47 GMT
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
	-	`sha256:3cf6607b465ef57028895e34149560cda1b504a743805be72b78b69bd9d13a97`  
		Last Modified: Tue, 29 Mar 2022 10:44:23 GMT  
		Size: 10.8 MB (10790925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8038d5fb4cdf9174619482d8ae95f2bd4c7afee6cd6b87c39b655828528f8523`  
		Last Modified: Tue, 29 Mar 2022 10:44:20 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544bb92eb1a7fbbc55ab90b5ae419ab5f3a14db9e01efc9b1453a2d73f7230e8`  
		Last Modified: Tue, 29 Mar 2022 10:44:55 GMT  
		Size: 10.3 MB (10316249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6333520d27e5a01c4c9ba3710f71bf15e578e3057feda793785d2e3073dc60c`  
		Last Modified: Tue, 29 Mar 2022 10:44:48 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3575edaca54892de40327920c32445a3fd1a4a206acd7be1370620434a5ca7a`  
		Last Modified: Tue, 29 Mar 2022 10:44:48 GMT  
		Size: 18.3 KB (18309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1dc97a4e537c66da48f1faf8813da1a2d6d89e13c7df599b9e7a1a3609e897`  
		Last Modified: Tue, 29 Mar 2022 10:44:48 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567a086a9337e20af68e811bfcbde4a6ac15adbcc61110e0f9773d2f991b15cd`  
		Last Modified: Tue, 29 Mar 2022 14:16:46 GMT  
		Size: 1.8 MB (1827614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012804f428290b6871abd88266fb7f7528f861803006032c1152b80d3560d6dd`  
		Last Modified: Tue, 29 Mar 2022 14:16:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa08f8955ebff6948b3cc949c860acf362b04b08bee63d0b367d4ca7ef3b0dd6`  
		Last Modified: Mon, 04 Apr 2022 22:24:02 GMT  
		Size: 660.1 KB (660102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd9a3de304bab00efa5168b28bede10e1a2b130c3d445c00f89bf4172ff70c1`  
		Last Modified: Mon, 04 Apr 2022 22:24:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe3c948486234be2246694914b458043d9b2a74213c98f39dd98183693c643`  
		Last Modified: Mon, 04 Apr 2022 22:24:30 GMT  
		Size: 20.9 MB (20937743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:77061f91eb2897e0da1be1164bd11b202c0c9dea787c0e195f2eff73fc10654c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50514905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb61feb1af6f9df07cd0e506c9f8473bde0b36eee566c8d3408d173ff8c00eb1`
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
# Tue, 29 Mar 2022 04:00:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 04:00:43 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 04:00:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 04:00:45 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 04:00:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 04:00:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:14:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 04:14:10 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:14:11 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 04:14:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 04:14:13 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 04:14:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 04:14:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 04:14:16 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 04:14:17 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 15:24:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 15:24:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:23:49 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:23:49 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:23:50 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:24:02 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:24:04 GMT
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
	-	`sha256:531483502f9533729551375df86ef71d5efcdda41acbb523290056aa95c4ca3e`  
		Last Modified: Tue, 29 Mar 2022 05:40:08 GMT  
		Size: 10.8 MB (10790720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d40d065ce8f0f6221f08e81c8ab46e08918bcc16d0df04bc68a1c0ad9b679e4`  
		Last Modified: Tue, 29 Mar 2022 05:40:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bde82771be39880a73b5434a660ee8325755058b1ebde90af24013f2d4a172`  
		Last Modified: Tue, 29 Mar 2022 05:40:29 GMT  
		Size: 11.5 MB (11530181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68103675f5d7fe9a1f977450b175d7b3e08fb3c4db217fec590bd1f3002efb08`  
		Last Modified: Tue, 29 Mar 2022 05:40:27 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722914d40ee15cd21f6d41db51f401d8a2a26ed28f4e11f9d9cbfe7415dd2b6e`  
		Last Modified: Tue, 29 Mar 2022 05:40:26 GMT  
		Size: 18.3 KB (18260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cb3bb202f586982eac1f7473dd6092d146b425475c37fa6bab4821b34e4a57`  
		Last Modified: Tue, 29 Mar 2022 05:40:26 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fc2de7cf883eeb2d576f733ac14ace15c3a4b39bd5716a2dd798214448e1da`  
		Last Modified: Wed, 30 Mar 2022 15:54:05 GMT  
		Size: 2.1 MB (2146714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcbccb9f2b578cbe262fb149b77ffadd6e13832ec0bbcd8c799cbb20c594620`  
		Last Modified: Wed, 30 Mar 2022 15:54:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4f83fad56954e6b608c419308c598a525d4389c343c632ad13ac789aed56a0`  
		Last Modified: Mon, 04 Apr 2022 22:18:08 GMT  
		Size: 660.1 KB (660106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18271e95bc20669ab7b76dbc22f92c2fc4d956771a448762f3b43a795762635`  
		Last Modified: Mon, 04 Apr 2022 22:18:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aef8842dbb1ef7727b111124a300b54ce2612853f601639f5bea7c9ff6effb`  
		Last Modified: Mon, 04 Apr 2022 22:18:13 GMT  
		Size: 20.9 MB (20938300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; 386

```console
$ docker pull drupal@sha256:f5ab60679beab92dca0141ad91b3032a6ea98a64c13319aab65e634a45b1f73e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51959319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ef36a124127cc1f6f4089ff6e59904742798359c59143ec2f8745b267ac9b63`
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
# Tue, 05 Apr 2022 00:44:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 05 Apr 2022 00:44:59 GMT
ENV PHP_VERSION=8.0.17
# Tue, 05 Apr 2022 00:45:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 05 Apr 2022 00:45:01 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 05 Apr 2022 00:45:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:51:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:51:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:51:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:51:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:51:59 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:52:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:52:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:52:02 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:52:03 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 07:40:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 07:40:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 07:40:45 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:40:45 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 07:40:46 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 07:40:58 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 07:40:59 GMT
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
	-	`sha256:2757fac8c2f9da893c5dca40b0a59a0445c03b0419ef8caff8186865330a7890`  
		Last Modified: Tue, 05 Apr 2022 01:30:17 GMT  
		Size: 10.8 MB (10790705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518ac3b606d3688529a317f42f785c5ba5cc7ef216843031f9ea43117a6effc5`  
		Last Modified: Tue, 05 Apr 2022 01:30:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8f73460ba6f78b080d83994d075e4e7a24e7ca1130d012b1acf3baefcff22`  
		Last Modified: Tue, 05 Apr 2022 01:30:38 GMT  
		Size: 12.3 MB (12286902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fbb7e3c9250f4843a9a01ab47acdd90a7f9b58aca86decac5f166942effe7a`  
		Last Modified: Tue, 05 Apr 2022 01:30:36 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6097d1a418dca2e6fb99c6ea3f9816aca7a5aefdb5374c9ceb84350071b17fc`  
		Last Modified: Tue, 05 Apr 2022 01:30:36 GMT  
		Size: 18.2 KB (18237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75152011c5eaac3e6aa4e1d2ae2e42f863d529f0b16b32f3b057cf53fb242ca2`  
		Last Modified: Tue, 05 Apr 2022 01:30:36 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdecae8f981367bdf1a57f32b3ef133af38c8b675a9655ca7893c8731be6511`  
		Last Modified: Tue, 05 Apr 2022 07:57:09 GMT  
		Size: 2.6 MB (2629378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e7132b76f03fa514528b46e78e3d980b6b73800f896fe2450a223db8e592d`  
		Last Modified: Tue, 05 Apr 2022 07:57:09 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4877d40685e9bd761fdb7f8a7f286b4f939dde90a33f1d88419cf5fe19ab0d3`  
		Last Modified: Tue, 05 Apr 2022 07:57:09 GMT  
		Size: 660.1 KB (660091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f54676616534ded8682b96d3b271039df9960494967b1bbd1154fedc18cd504`  
		Last Modified: Tue, 05 Apr 2022 07:57:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fb0f2d7284e53152997efb6b0e3699152f8f33568da2505dbd500a6450ec9d`  
		Last Modified: Tue, 05 Apr 2022 07:57:14 GMT  
		Size: 20.9 MB (20938199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; ppc64le

```console
$ docker pull drupal@sha256:fd192a654f804052359e0ee04da471fcccf2d228110efb7761d42320c0a09fa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51749356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53e9306be110ee559a3d66a52fbc877bd72f95f7b273c1d64b7bc0235ec19894`
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
# Tue, 29 Mar 2022 03:33:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 29 Mar 2022 03:33:16 GMT
ENV PHP_VERSION=8.0.17
# Tue, 29 Mar 2022 03:33:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 29 Mar 2022 03:33:19 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 29 Mar 2022 03:33:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 03:33:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:43:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:43:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:44:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:44:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:44:07 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:44:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 03:44:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 03:44:17 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 03:44:19 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 18:33:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 18:33:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 22:15:05 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 22:15:09 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 22:15:11 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 22:15:45 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 22:15:52 GMT
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
	-	`sha256:d9ee6ff7f6f3bcbabbd93af19acfd46df0a1f157f51d5c57d8c03bdece0d2655`  
		Last Modified: Tue, 29 Mar 2022 05:18:51 GMT  
		Size: 10.8 MB (10790950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243525eb4f6327cfed261508e573568de5e4054ecf79c68b92971d42d3ce49e6`  
		Last Modified: Tue, 29 Mar 2022 05:18:49 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6529682d42737786d134264fb11290b60f070eed5d9c8e32efff568e1f083c1`  
		Last Modified: Tue, 29 Mar 2022 05:19:16 GMT  
		Size: 12.4 MB (12448598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b5e9a9ce7465b78c259f632e3963eb13e6e55f38e80697dd8364d78ea1a8d5`  
		Last Modified: Tue, 29 Mar 2022 05:19:13 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49546c5c4f863966099e15507a5b6d7b0114777c07f25152e3f2d2ca2c4cd83`  
		Last Modified: Tue, 29 Mar 2022 05:19:14 GMT  
		Size: 18.3 KB (18339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41b0753813f5d82bca6ee4d4ff1d972e2031724cea4f6a93512ed61997319c2`  
		Last Modified: Tue, 29 Mar 2022 05:19:13 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ba1f9488ae38d70937bb60fe65d48ea3d738e4a5229d5f19a82025695278a4`  
		Last Modified: Wed, 30 Mar 2022 20:08:38 GMT  
		Size: 2.3 MB (2317791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34065bd05f320dc2bf6cca9b9e00dced5dd0b47e1268b37145deff1d7a65c836`  
		Last Modified: Wed, 30 Mar 2022 20:08:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8d3d44ae36b0f45aff957fc0b1c6671bafa78e8a26918e4bc8b4f3cb76f135`  
		Last Modified: Mon, 04 Apr 2022 23:10:13 GMT  
		Size: 660.1 KB (660102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1d4f68a094d83acad03484f305468d2c08b54653e9b32dd1315a1eb02cd6ea`  
		Last Modified: Mon, 04 Apr 2022 23:10:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fc263fe4557ffebd05d2b3e409556c9e964aa2715391a1bffbe2ebe4b69e2b`  
		Last Modified: Mon, 04 Apr 2022 23:12:01 GMT  
		Size: 20.9 MB (20937673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.14` - linux; s390x

```console
$ docker pull drupal@sha256:ca778b0a08aa5ccbc32f22955d8343176762ae23000a2a26475018866f0a5eef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50266519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1f88026c7119720f0e5b11029d8e9810a0561a05dcb6feddd4c5a6a15c43edf`
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
# Tue, 05 Apr 2022 00:35:17 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 05 Apr 2022 00:35:17 GMT
ENV PHP_VERSION=8.0.17
# Tue, 05 Apr 2022 00:35:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Tue, 05 Apr 2022 00:35:18 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Tue, 05 Apr 2022 00:35:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:35:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:41:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:41:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:41:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:41:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:41:15 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:41:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:41:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:41:16 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:41:17 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:50:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:50:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:50:57 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:50:58 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 11:50:58 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:51:10 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:51:14 GMT
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
	-	`sha256:e47b38aaf5ea775d7d01bdbb682499b9d4a2dd4f10fefe57fb713894d5cabeff`  
		Last Modified: Tue, 05 Apr 2022 02:54:05 GMT  
		Size: 10.8 MB (10790961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f068a159721a053b161cd24e14e14b6be17258c44862b25cddda377fd165591`  
		Last Modified: Tue, 05 Apr 2022 02:54:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af46336e0cd2dd3f5a625f66b4a55e33474a1950ed6caf2988ce885741ec11c8`  
		Last Modified: Tue, 05 Apr 2022 02:54:19 GMT  
		Size: 11.3 MB (11298091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a5c0e1ec3adc6aea637d4c5827ebfd33ea514b2cf69e76a34d66aaef22c4d9`  
		Last Modified: Tue, 05 Apr 2022 02:54:18 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b0e6b7dff138c57d8ba55ca7dda9b7ed9c74ede7f76b57c528a9f76dc09aca`  
		Last Modified: Tue, 05 Apr 2022 02:54:18 GMT  
		Size: 18.4 KB (18369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03b34298dccba63b18946c8b59d06261ddf262facdd48d059756c95fb07d09a`  
		Last Modified: Tue, 05 Apr 2022 02:54:18 GMT  
		Size: 8.6 KB (8567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef9cbe3ca5444ee9c042463be609d0bc6ee235c3ab69eaa5a4bf48f9002b8b3`  
		Last Modified: Tue, 05 Apr 2022 12:08:10 GMT  
		Size: 2.2 MB (2181397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b7e8fca36e899eb588c63de14c7feabf40df646d2fc0f61324dfa9ca4cf6b`  
		Last Modified: Tue, 05 Apr 2022 12:08:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83f06a74af80c9952b2806128e6804578a2641e60410cb5c1b9b392b32bfb7`  
		Last Modified: Tue, 05 Apr 2022 12:08:10 GMT  
		Size: 660.1 KB (660096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974c6b63543eeddd975af7db22f5680835ec4ef9ff757fd467e4e55142c36113`  
		Last Modified: Tue, 05 Apr 2022 12:08:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd32ca21bdbc86d1d61e24c09512ba4720e34da271f94efaae1676761768f31`  
		Last Modified: Tue, 05 Apr 2022 12:08:14 GMT  
		Size: 20.9 MB (20937293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
